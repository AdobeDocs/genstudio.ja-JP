---
title: 有効なプロンプトの記述
description: パフォーマンスマーケティング用の Adobe GenStudio の効果的なプロンプトを記述する方法について説明します。
feature: Prompt, Generative AI, Brands Service, Personas Service, Products Service, Guidelines
exl-id: 0cd4db4f-d031-4c1f-a4e7-adc220f947fc
source-git-commit: bd3c5c9ff12c962d4123ac992fb74cd94e184172
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 2%

---

# 有効なプロンプトの記述

Adobe GenStudio for Performance Marketingで効果的に作業するには、生成 AI とのコミュニケーションが不可欠です。

GenStudio for Performance Marketingでは、アセットを変更する機会があるたびに生成 AI プロンプトが表示されます。 効果的なプロンプトのコンポーネントには、説明的な言語、例、設定済みのガイドラインでは提供されない情報を含める必要があります。

ベストプラクティスとしては、[ ガイドライン ](/help/user-guide/guidelines/overview.md) を使用してGenStudio for Performance Marketingにブランド情報を提供すると、生成 AI を最大限に活用して、ブランドに合わせたコンテンツエクスペリエンスを作成できます。

## 記述言語

自然言語を使用して、アイデアを明確に表現し、エクスペリエンスを作成できます。 プロンプトは、パーソナライズされたチャネルコンテンツやビジョンを補完する画像を生成するために AI をガイドします。 提供する詳細情報が多いほど、ニーズを満たす画像やエクスペリエンスを作成する可能性が高くなります。 明確で説明的な言語を使用して、可能な限り詳細な情報を提供します。

- **画像** には、雰囲気、気分、色、構成、スタイルを説明する単語を使用します。
- **コピー** については、オーディエンス、目的、新機能の説明、例およびアクションを説明する単語を使用します。

インテント、ターゲットオーディエンスおよびスタイルに関する情報を明確にするサンプルプロンプトを次に示します。

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.
```

+++サンプル結果を参照

![ 生成された 3 通のメール ](/help/assets/sample-email.png)

+++

## プロンプト条件

GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) では、プロンプト領域で **[!UICONTROL プロンプト条件]** （[_パラメーター_](/help/user-guide/create/overview.md#parameters) とプロンプト）を使用して、AI の解釈を改善するために選択を通じて詳細を追加できます。

[ メール ](/help/user-guide/create/email-experiences.md) の場合、プロンプト条件には [ パラメーター ](/help/user-guide/guidelines/overview.md) に _ガイドライン_ を追加すること、メールのバリエーションで使用するアセットをアップロードすること、説明プロンプトを含めることができます。 [ メタ広告 ](/help/tutorials/create-meta-ad.md) の場合、プロンプト条件には、_パラメーター_ でのブランドガイドライン、既存アセットの選択またはアップロード、画像またはアセットに関連する設定（縦横比など）、プロンプトなどが含まれます。 真のパワーは、[ ガイドラインの設定 ](/help/user-guide/guidelines/add-guidelines.md) から始まります。

>[!NOTE]
>
>プロンプト領域の _パラメータ_ にガイドラインが追加されている場合は、プロンプトにガイドラインへの参照を含める必要はありません。 GenStudio for Performance Marketingでは、これらの [!DNL Brands]、[!DNL Products] および [!DNL Personas] をコンテンツの生成に活用します。

### ガイドライン

GenStudio for Performance Marketingのガイドラインは、生成 AI がアセット構成をパーソナライズするのに役立ちます。 プロンプト条件が表示されたら、設定済みのガイドラインから [[!DNL Brand]](/help/user-guide/guidelines/brands.md)、[[!DNL Persona]](/help/user-guide/guidelines/personas.md)、[[!DNL Product]](/help/user-guide/guidelines/products.md) を選択できます。

>[!TIP]
>
>GenStudio for Performance Marketingで [!DNL Brand] ガイドラインを使用する方法とタイミングを制御します。 ブランドガイドラインの設定および管理方法については、[ ガイドライン ](/help/user-guide/guidelines/overview.md) を参照してください。

### 構造化されたプロンプト

複数セクションのメールの場合、[ メール ](/help/user-guide/create/email-experiences.md) 内のセクションごとに異なるコンテンツを生成するためのセクション固有の手順を提供するように促す構造を作成できます。 構造化プロンプトは、生成されたコンテンツを対応するコンテンツプレースホルダーに挿入できるように ](/help/user-guide/content/email-template.md#multi-section-emails) メールテンプレート内のセクション名 [ を直接参照する必要があります。

例えば、メールの 1 番目のセクションで新製品を宣伝するコンテンツを作成し、2 番目のセクションで製品のコスト削減メリットの詳細を説明するコンテンツを作成するようにGenStudio for Performance Marketingに指示できます。

構造化されたプロンプトでは、次の操作を行う必要があります。

- メールテンプレートのセクション名に、次のいずれかの参照を使用します。
   - ポッド
   - グループ
   - セクション
   - モジュール

  例えば、テンプレートでセクション名として `moduleA` または `Group-3` を使用している場合、プロンプトでこれらのセクション名を参照できます。

- 推奨されるルール/構造に従います。 プロンプト構造が指定された形式に準拠していない場合、プロンプトは *すべて* のメールセクションに適用され、引き続きコンテンツの生成を容易にします。
- [ メールテンプレートで定義した ](/help/user-guide/content/email-template.md#code-an-email-template) セクション名を使用します。 プロンプト参照は、メールテンプレートにコーディングされたセクション名と一致する必要があります。
- 大文字と小文字を区別しない。 例えば、メールテンプレートと構造化プロンプトで `Pod` または `pod` を使用できます。
- 最初に汎用のユーザープロンプトを参照し、次にセクション固有のディレクティブを参照します。
- セクション名の参照とディレクティブの間の区切りとして、コロン、ハイフン、コンマ、その他の区切り文字（`,:;#$!~|@=-%&*^_`）を使用します。 例えば、次をセクション固有のプロンプトディレクティブとして使用できます。`Pod1; Describe how to easily edit text and swap images.`

以下は、推奨されるプロンプト構造を明確にし、`Pod1`、`Pod2`、`Pod3` などの識別用語 `Pod` を使用するメールテンプレートを活用するプロンプトのサンプルです。

```properties
Create an exciting multi-pod email focusing on Creative Cloud and its powerful generative AI capabilities.

Encourage customers to convert to Photoshop or use a free Photoshop trial. We want to better educate them about app features.

Pod1: Focus on Adobe Photoshop and its new generative AI tools that enable creators to bring images to life in minutes.

Pod2: Focus on Adobe Illustrator and its new generative AI tools, such as Generative Shape Fill, which allows you to quickly fill your vector outline and explore a variety of options that match the look and feel of your own artwork.

Pod3: Focus on Adobe Acrobat Pro. Make users aware that with Acrobat Pro they can edit images and text inside a PDF.
```

[ メールテンプレートの準備 ](/help/user-guide/content/email-template.md#code-an-email-template) を参照してください。

## 再試行

プロンプトは反復的なプロセスです。 結果が期待どおりでない場合は、プロンプトを確認し、変更を加えるか、詳細を追加します。 または、キャンペーン概要のセクションにペーストすることもできます。 特定の単語、要素またはテーマを避けるようにGenStudio for Performance Marketingにリクエストすることもできます。

## ベストプラクティス

効果的なプロンプトを作成するためのシンプルなベストプラクティス：

- 具体的に説明し、実行する操作と実行しない操作の詳細を指定します。
- 外部参照を使用してコンテキストを提供する
- GenStudio for Performance Marketingのガイドラインを活用します。
- ガイドラインを定期的に確認し、調整します。
- 繰り返して調整します。
- 実験を通じて学ぶ。
