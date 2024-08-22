---
title: テンプレートのカスタマイズ
description: パフォーマンスマーケター向けのAdobe GenStudio用カスタムテンプレートを作成する方法について説明します。
level: Intermediate
feature: Templates, Content
source-git-commit: 44390d551e638fcff47cff5844fcfda4ed9f98f3
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# テンプレートのカスタマイズ

_Handlebars_ テンプレート言語を使用して、パフォーマンスマーケター向けにAdobe GenStudio用のHTMLテンプレートを調整します。 Handlebars 構文では、コンテンツプレースホルダーとして二重中括弧を使用した通常のテキストを使用します。 テンプレートの準備方法については、_Handlebars 言語ガイド_ の [`What is Handlebars?`](https://handlebarsjs.com/guide/#what-is-handlebars) を参照してください。

GenStudio for Performance Marketers で使用するHTMLテンプレートがない場合は、まず、HTMLタグ（`DOCTYPE`、`html`、`head` および `body`）を使用してテンプレートの構造を定義できます。 次に、外観をカスタマイズするための CSS スタイルを含む、基本的なメールテンプレートを示します。

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
>次のいくつかの節では、メールフィールドのコンテンツプレースホルダーを追加します。例テンプレート、不要な要素をプレビューから非表示、静的コンテンツへのリンクの管理を参照してください。 テンプレートの準備が整ったら、[ パフォーマンスマーケター向けにGenStudioにアップロード ](use-templates.md#upload-a-template) し、カスタムテンプレートに基づいてパーソナライズされたメールの生成を開始できます。

## コンテンツプレースホルダー

テンプレートの先頭または本文内では、Handlebars 構文を使用して、コンテンツプレースホルダーを挿入できます。この場合、パフォーマンスマーケターがテンプレートに実際のコンテンツを入力するGenStudioが必要です。 GenStudio for Performance マーケターは、フィールド名に基づいてコンテンツプレースホルダーを認識し、解釈します。

例えば、`{{ headline }}` を使用して、メールのヘッドラインを配置する場所を指定できます。

```handlebars
<div>{{ headline }}</div>
```

### 認識されたフィールド名

カスタムテンプレートで許可されるフィールドの最大数は 20 です。

次の表に、テンプレートへの母集団について、GenStudioのパフォーマンスマーケター向けに認識されるフィールド名を示します。

| フィールド | 役割 | チャネルテンプレート |
| -------------- | ---------------------- | -------------------- |
| `pre_header` | プリヘッダー | 電子メール （推奨） |
| `headline` | 見出し | メール（推奨） <br> メタ広告 |
| `body` | 本文コピー | メール（推奨） <br> メタ広告 |
| `cta` | コールトゥアクション | メール（推奨） <br> メタ広告 |
| `on_image_text` | 画像テキスト上 | メタ広告（推奨） |
| `image` | 画像 | メール（推奨） <br> メタ広告（推奨） |
| `brand_logo` | 選択したブランドのロゴ <br> 推奨使用については、[ フィールド名 ](#brand-logo-field-name) を参照してください。 | メールメ <br> タ広告 |

GenStudio for Performance マーケターは、特定のフィールドをテンプレートに自動的に入力するので、テンプレートデザインに含める必要はありません。

- `subject` フィールド （メールテンプレート）
- `headline`、`body`、`CTA` の各フィールド（メタ広告テンプレート）

>[!WARNING]
>
>instagram広告の場合、生成されたヘッドラインは最終的なエクスペリエンスには表示されません。

#### ブランドロゴフィールド名

次の例は、ブランドロゴの条件付きレンダリング、ソースの検証、ブランドロゴが使用できない場合にデフォルトまたは代替ロゴを提供、スタイルを適用する 2 つの方法を示しています。

_例_:HTML `img src` 定義

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;"> 
```

_例_:Handlebars 条件内

```handlebars
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

#### 手動フィールド名

その他のすべてのフィールド名は、手動で入力されたフィールドとして扱われます。 編集可能なセクションを作成するには、セクション名の周りに二重括弧を追加します。

```handlebars
{{customVariable}}
```

## セクションまたはグループ

_セクション_ このセクションのフィールドには高い一貫性が必要であることをパフォーマンスマーケター向けにGenStudioに伝えます。 この関係を確立すると、AI がセクションのクリエイティブ要素に一致するコンテンツを生成するのに役立ちます。

フィールド名に任意の接頭辞を使用して、フィールドがセクションまたはグループの一部であることを示します。

例えば、ハイライトされた領域に表示されるコンテンツにスポットライトを当てることができます。

- `spotlight_headline`
- `spotlight_body`

各セクションには、各フィールドタイプを 1 つだけ含めることができます。 上記の例では、`spotlight` プレフィックスに `spotlight_headline` フィールドを 1 つだけ含めることができます。

テンプレートには、最大で次の 3 つのセクションを含めることができます。

- `headline`
- `body`
- `spotlight_headline`
- `spotlight_body`
- `news_headline`
- `news_body`

パフォーマンスマーケター向けGenStudioでは、`spotlight_headline` は `news_body` よりも `spotlight_body` と密接に関係していることを理解しています。

## テンプレートの例

+++例：1 つのセクションを持つメールテンプレート

次に、1 つのセクションを含むメールのHTMLテンプレートの基本的な例を示します。 ヘッドには、スタイル設定用のシンプルなインライン CSS が含まれています。 本文には、`pre-header`、`headline`、`image` [ プレースホルダー ](#content-placeholders) が含まれており、GenStudio for Performance マーケターがメール生成プロセス中にコンテンツを挿入するために使用します。

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

+++例：複数のセクションを持つメールテンプレート

以下は、上記の例と同じHTMLテンプレートですが、さらに 2 つのセクションがあります。 ヘッドには、グループのスタイル設定に使用するインライン CSS が含まれています。 本文では、プレフィックスを使用して、[ コンテンツプレースホルダー ](#content-placeholders) を含む 2 つのグループを使用します。

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

+++例：メタ広告テンプレート

次に、メタ広告テンプレートの基本的な例を示します。 ヘッドには、スタイル設定用のインライン CSS が含まれています。 本文では、プレフィックスを使用して [ コンテンツプレースホルダー ](#content-placeholders) を使用します。

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">"{{ headline }}"</div>
    <div class="ad-body">"{{ body }}"</div>
    <a href="(https://example.com)" class="ad-cta">"{{ CTA }}"</a>
</div>
</body>
</html>
```

+++

## テンプレートのプレビュー

組み込みヘルパー（特定のアクションを実行する Handlebars テンプレート言語の特別な式）を使用して、特別なコンテンツの表示を制御します。 例えば、プレビューリンクをクリーンに保ちながら、書き出されたテンプレート内のリンクにトラッキングパラメーターを追加できます。

テンプレートのレンダリング時には `_genStudio.browser` の値が設定され、テンプレートの書き出し時には `genStudio.export` の値が設定されます。 条件付きラッパーを使用して、メールの上部に特定のコンテンツを含めることもできます。例えば、テンプレートを書き出しに使用する場合です。

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

もう 1 つの例として、GenStudioでテンプレートをプレビューする際に、トラッキングコードを使用しないようにすることがあります。 次の例では、プレビューリンクをクリーンな状態に保ちながら、書き出されたテンプレート内のリンクにトラッキングパラメーターを追加する方法を示します：

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## 静的コンテンツ

メールおよびメタテンプレートは、多くの場合、パフォーマンスマーケター向けにGenStudioの外部でホストされている画像や CSS ファイルにリンクされています。 GenStudio for Performance マーケターが、これらのテンプレートまたはから派生したエクスペリエンスのサムネールを生成する際、正しいクロスオリジンリソース共有（CORS）ヘッダーがない場合、これらの外部リソースが無視される場合があります。

サムネール生成プロセスの実行中にこれらのリソースを使用できるようにするには、次の 2 つのオプションを検討します。

1. **CORS ヘッダーを使用**：ホストサーバーは、実稼動環境の値に設定された `Access-Control-Allow-Origin` ヘッダーで応答 `https://experience.adobe.com` 送信する必要があります。 これにより、パフォーマンスマーケターはGenStudioからリソースにアクセスして組み込むことができます。
1. **データ URL を使用**：データ URL を使用して、外部リソースをテンプレートに直接埋め込みます。 この方法では、CORS の制限をバイパスし、サムネールの生成中にリソースを利用できるようにします。
