---
title: テンプレートのカスタマイズ
description: GenStudioのカスタムテンプレートを作成する方法を説明します。
level: Intermediate
feature: Templates, Content
source-git-commit: 423956d6fdbf5b31041d44eb434f90d55a87d7c0
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---


# テンプレートのカスタマイズ

_Handlebars_ テンプレート言語を使用して、GenStudio用のHTMLテンプレートを調整できます。 Handlebars 構文では、コンテンツプレースホルダーとして二重中括弧を使用した通常のテキストを使用します。 テンプレートの準備方法については、_Handlebars 言語ガイド_ の [`What is Handlebars?`](https://handlebarsjs.com/guide/#what-is-handlebars) を参照してください。

## テンプレート構造

<!-- This is for email. In the future, maybe use tabs to provide guidance for other template types.
-->

GenStudioで使用するHTMLテンプレートが準備されていない場合は、まず、HTMLタグ `DOCTYPE`、`html`、`head` および `body` を使用してメールの構造を定義できます。 CSS スタイルを含めて、メールの外観をカスタマイズできます。

```html
<!DOCTYPE html>
<html>
<head>
    <title>Title</title>
    <style>
    </style>
</head>
<body>
</body>
</html>
```

>[!TIP]
>
>次のいくつかの節では、メールフィールドのコンテンツプレースホルダーを追加し、不要な要素をプレビューから非表示にし、静的コンテンツへのリンクを管理します。 テンプレートの準備が整ったら、[GenStudioにアップロード ](use-templates.md#upload-a-template)、カスタムテンプレートに基づいてパーソナライズされたメールの生成を開始できます。

## コンテンツプレースホルダー

テンプレートの先頭または本文内では、ハンドルバー構文を使用して、GenStudioでメールに実際のコンテンツを入力する必要があるコンテンツプレースホルダーを挿入できます。 GenStudioは、フィールド名に基づいてコンテンツプレースホルダーを認識し、自動的に解釈します。

例えば、`{{ headline }}` を使用して、メールのヘッドラインを配置する場所を指定できます。

```handlebars
<div>{{ headline }}</div>
```

カスタムテンプレートで許可されるフィールドの最大数は 20 です。

**認識されたフィールド名**:

| フィールド | 役割 | チャネルテンプレート |
| -------------- | ---------------------- | -------------------- |
| `pre_header` | プリヘッダー | email |
| `headline` | 見出し | メールソ <br> シャル広告 |
| `body` | 本文コピー | メールソ <br> シャル広告 |
| `cta` | コールトゥアクション | メールソ <br> シャル広告 |
| `on_image_text` | 画像テキスト上 | ソーシャル広告 |
| `image` | 画像 | メールソ <br> シャル広告 |
| `brand_logo` | 選択したブランドのロゴ | ソーシャル広告 |

>[!IMPORTANT]
>
>GenStudioは、[!DNL Create] ールプロセス中にメールテンプレートに `subject` フィールドを自動的に提供するので、メールテンプレートに「件名」フィールドを含める必要はありません。

+++例：基本テンプレート

次に、メールのHTMLテンプレートの基本的な例を示します。 ヘッドには、スタイル設定用のシンプルなインライン CSS が含まれています。 本文には、`pre-header`、`headline` および `image` プレースホルダーが含まれており、メール生成プロセス中にGenStudioでコンテンツを挿入するために使用されます。

```handlebars {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

### 背景画像

Meta 用に広告をデザインする場合は、テキストとブランドロゴオーバーレイで補完される背景画像を使用することが重要です。 画像の適切な拡大縮小を保証するために、メタ広告テンプレートでは `aspect ratio` を指定する必要があります。 このコンテキストでは、1 つの画像フィールドのみを指定できます。

## セクションまたはグループ

_セクション_ セクションに属するフィールドには高度なコヒーレンスが必要であることをGenStudioに通知する手段を提供します。 この関係を確立すると、AI がセクションのクリエイティブ要素に一致するコンテンツを生成するのに役立ちます。 テンプレートには、最大 3 つのセクションを含めることができます。

フィールド名に任意の接頭辞を使用して、このフィールドがセクションまたはグループの一部であることを示します。 例えば、ハイライトされた領域に表示されるコンテンツにスポットライトを当てることができます。 この領域のコンテンツを、共通のプレフィックスで識別するように選択できます。

- `spotlight_headline`
- `spotlight_body`

各セクションは、1 つのフィールドタイプを 1 つだけ持つことができます。 例えば、上記の `spotlight` プレフィックスが付いたサンプル グループでは、`spotlight_headline` フィールドを 1 つだけ持つことができます。

複数のセクションがある場合（最大 3 つ）:

- `headline`
- `body`
- `spotlight_headline`
- `spotlight_body`
- `news_headline`
- `news_body`

GenStudioは `spotlight_headline` が `news_body` よりも `spotlight_body` と密接に関係していることを理解しています。

+++例：複数のセクションを持つテンプレート

以下は、上記の例と同じHTMLテンプレートですが、さらに 2 つのセクションがあります。 ヘッドには、ポッドのスタイルを設定するためのインライン CSS が含まれています。 本文では、プレフィックスを使用してコンテンツプレースホルダーを持つ 2 つのポッドを使用します。

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
        .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
        }
        .pod h2 {
            color: #333;
        }
        .pod p {
            color: #666;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
        <div class="pod">
            <h2>{{ pod1_headline }}</h2>
            <p>This is Pod 1 content.</p>
        </div>
        <div class="pod">
            <h2>{{ pod2_headline }}</h2>
            <p>This is Pod 2 content.</p>
        </div>
    </div>
</body>
</html>
```

+++

## テンプレートのプレビュー

メールテンプレートには、GenStudioでプレビューする必要のない特別なコンテンツが含まれている場合があります。 組み込みのヘルパーを使用して、このコンテンツの表示を制御できます。このヘルパーは、Handlebars テンプレート言語の特別な式で、特定のアクションの実行に役立ちます。

テンプレートのレンダリング時には `_genStudio.browser` の値が設定され、テンプレートの書き出し時には `genStudio.export` の値が設定されます。 条件付きラッパーを使用して、メールの上部に特定のコンテンツを含めることもできます。例えば、テンプレートを書き出しに使用する場合です。

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

もう 1 つの例として、GenStudioでメールテンプレートをプレビューする際に、トラッキングコードを使用できないようにすることがあります。 次の例では、プレビューリンクをクリーンな状態に保ちながら、書き出されたテンプレート内のリンクにトラッキングパラメーターを追加する方法を示します：

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## 静的コンテンツ

多くの場合、メールおよびメタテンプレートは、GenStudioの外部でホストされる画像や CSS ファイルにリンクされています。 GenStudioがこれらのテンプレートまたはそれらから派生したエクスペリエンスのサムネールを生成する際、正しいクロスオリジンリソース共有（CORS）ヘッダーがない場合、これらの外部リソースが無視される場合があります。

サムネール生成プロセスの実行中にこれらのリソースを使用できるようにするには、次の 2 つのオプションを検討します。

1. **CORS ヘッダーを使用**：ホストサーバーは、実稼動環境の値に設定された `Access-Control-Allow-Origin` ヘッダーで応答 `https://experience.adobe.com` 送信する必要があります。 これにより、GenStudioはリソースにアクセスして含めることができます。
1. **データ URL を使用**：データ URL を使用して、外部リソースをテンプレートに直接埋め込みます。 この方法では、CORS の制限をバイパスし、サムネールの生成中にリソースを利用できるようにします。
