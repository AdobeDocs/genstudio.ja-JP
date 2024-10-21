---
title: メールエクスペリエンス
description: Adobe GenStudio for Performance Marketingでのメールエクスペリエンスについて説明します。
feature: Experiences, Content Generation, Create, Generative AI, Variant Generation
role: User
level: Beginner
source-git-commit: 6ba029f46a37c159ec48676a158a6a9b8fb5465d
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# メールエクスペリエンス

Adobe GenStudio for Performance Marketingでは、ジェネレーティブ AI を使用して [ 効果的なメールエクスペリエンスの作成 ](/help/tutorials/create-email-experience.md) を合理化できます。

[!DNL Create] を使用すると、最新のマーケターは [ ガイドライン ](/help/user-guide/guidelines/overview.md)、画像アセット、および [ 適切に作成されたプロンプト ](/help/user-guide/effective-prompts.md) を使用して、ブランドに合ったメールエクスペリエンスをすばやく [ 作成 ](/help/tutorials/create-email-experience.md) できます。

メールエクスペリエンスの編集可能なセクションには、次のものが含まれます。

* プリヘッダー
* 見出し
* 本文
* コールトゥアクション（CTA）
* 画像
* ブランドロゴ

[ テンプレート要素 ](/help/user-guide/content/use-templates.md#template-elements) を参照してください。

<!-- ## Email capabilities

Content creators and marketers can produce brand-consistent email experiences in GenStudio for Performance Marketing. -->

## 複数セクションのメール

メールエクスペリエンスには複数のセクションを含めることができるので、ブランドや目標に合わせて完全にカスタマイズできます。 [ [!DNL Products]  各セクションのアセットを選択して視覚的に表示し ](/help/tutorials/create-email-experience.md#add-parameters)[ 構造化プロンプト ](/help/user-guide/effective-prompts.md#structured-prompts) を使用して一意のコンテンツを作成します。 各セクションは、1 つのビジュアルアセットをサポートします。

複数セクションテンプレートの作成方法については、[ メールテンプレートの準備 ](/help/user-guide/content/email-template.md) を参照してください。

## プログレッシブロード

コンテンツ生成プロセスが開始すると、メールバリアント内の生成されたコンテンツの各セクションがキャンバスにプログレッシブに読み込まれます。 エクスペリエンス、アセット、エクスペリエンス内のフィールドとセクションは、生成されるとキャンバスに個別に表示されます。

「**[!UICONTROL 生成]**」をクリックすると、キャンバスの下部に読み込みインジケーターが表示され、生成の進行状況が更新されます。

メールエクスペリエンスの各フィールドとセクションは、次の順序で順に読み込まれます。

1. バリアント名
1. すべてのバリエーションの件名
1. プリヘッダー
1. 見出し、メール本文（単一セクションのメールの場合）、コールトゥアクション
1. 後続セクションのメール本文（複数セクションのメールの場合）
1. ブランドの検証プロセスが発生し、各バリアントに [_ブランドガイドラインチェック_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) が入力されます。
