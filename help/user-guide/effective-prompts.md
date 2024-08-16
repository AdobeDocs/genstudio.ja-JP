---
title: 有効なプロンプトの記述
description: パフォーマンスマーケター向けのAdobe GenStudioの効果的なプロンプトを記述する方法について説明します。
feature: Prompt, Generative AI, Brands Service, Personas Service, Products Service, Guidelines
source-git-commit: c9d09801f0bd3732611b01d4a98cc7ebf38884d7
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---


# 有効なプロンプトの記述

パフォーマンスマーケターがAdobe GenStudioに効果的に取り組むには、ジェネレーティブ AI とのコミュニケーションが不可欠です。

GenStudio for Performance マーケターは、アセットに変更を加える機会があるたびに生成 AI プロンプトを提供します。 効果的なプロンプトのコンポーネントには、説明的な言語、例、設定済みのガイドラインでは提供されない情報を含める必要があります。

ベストプラクティスとして、[ ガイドライン ](/help/user-guide/guidelines/overview.md) を使用して、パフォーマンスマーケター向けのGenStudioにブランド情報を提供すると、ジェネレーティブ AI を最大限に活用して、ブランドに合わせたコンテンツエクスペリエンスを作成できます。

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

GenStudio for Performance Marketers [[!DNL Create]](/help/user-guide/create/overview.md) では、プロンプト領域で **[!UICONTROL プロンプト条件]** （[_パラメーター_](/help/user-guide/create/overview.md#parameters) とプロンプト）を使用して、選択によって詳細を追加し、AI の解釈を改善できます。

[ メール ](/help/tutorials/create-email-experience.md) の場合、プロンプト条件には [ パラメーター ](/help/user-guide/guidelines/overview.md) に _ガイドライン_ を追加すること、メールのバリエーションで使用するアセットをアップロードすること、説明プロンプトを含めることができます。 [ メタ広告 ](/help/tutorials/create-meta-ad.md) の場合、プロンプト条件には、_パラメーター_ でのブランドガイドライン、既存アセットの選択またはアップロード、画像またはアセットに関連する設定（縦横比など）、プロンプトなどが含まれます。 真のパワーは、[ ガイドラインの設定 ](/help/user-guide/guidelines/add-guidelines.md) から始まります。

>[!NOTE]
>
>プロンプト領域の _パラメータ_ にガイドラインが追加されている場合は、プロンプトにガイドラインへの参照を含める必要はありません。 GenStudio for Performance マーケターは、これらの [!DNL Brands]、[!DNL Products] および [!DNL Personas] をコンテンツの生成に活用します。

### ガイドライン

GenStudio for Performance Marketers のガイドラインは、ジェネレーティブ AI がアセット構成をパーソナライズするのに役立ちます。 プロンプト条件が表示されたら、設定済みのガイドラインから [[!DNL Brand]](/help/user-guide/guidelines/brands.md)、[[!DNL Persona]](/help/user-guide/guidelines/personas.md)、[[!DNL Product]](/help/user-guide/guidelines/products.md) を選択できます。

>[!TIP]
>
>GenStudio for Performance Marketers で [!DNL Brand] ガイドラインを使用する方法とタイミングを制御します。 ブランドガイドラインの設定および管理方法については、[ ガイドライン ](/help/user-guide/guidelines/overview.md) を参照してください。

## 再試行

プロンプトは反復的なプロセスです。 結果が期待どおりでない場合は、プロンプトを確認し、変更を加えるか、詳細を追加します。 URL を例として、または詳しい情報のソースとして指定することで、プロンプトを絞り込むことができます。

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.

Use information from https://www.adobe.com/products/photoshop.html to inspire users with the latest features.
```

または、キャンペーン概要のセクションにペーストすることもできます。 GenStudio for Performance Marketer に対して、特定の単語、要素またはテーマを避けるようにリクエストすることもできます。

## ベストプラクティス

効果的なプロンプトを作成するためのシンプルなベストプラクティス：

- 具体的に説明し、実行する操作と実行しない操作の詳細を指定します。
- 外部参照を使用してコンテキストを提供する
- マーケターのパフォーマンスガイドラインにGenStudioを活用します。
- ガイドラインを定期的に確認し、調整します。
- 繰り返して調整します。
- 実験を通じて学ぶ。
