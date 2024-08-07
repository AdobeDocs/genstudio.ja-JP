---
title: メールエクスペリエンスの作成
description: Adobeでメールエクスペリエンスを作成する方法を説明します  [!DNL GenStudio]。
feature: Content, Brands Service, Guidelines, Content Generation
role: User
level: Beginner
type: Tutorial
recommendations: noDisplay
source-git-commit: fa89422db3e1679516a377c9bfd9f05ab6e63428
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 0%

---


# メールエクスペリエンスの作成

このチュートリアルでは、GenStudio [[!DNL Create]](/help/user-guide/create/overview.md) （左側のナビゲーションエリアの絵筆アイコン）を使用してブランドのメールエクスペリエンスを生成する方法を説明します。

効果的なメールエクスペリエンスを作成するには、開始する前に [GenStudioにガイドラインを追加 ](/help/user-guide/guidelines/add-guidelines.md) し、[ プロンプトの作成の基本 ](/help/user-guide/effective-prompts.md) をブラッシュアップすることをお勧めします。

## テンプレートを選択

新しいメールエクスペリエンスの作成を開始するには、使用可能なテンプレートを使用してコンテンツのフレームワークを提供します。

**メールテンプレートを選択するには**:

1. _[!DNL Create]_で、「今日は何を作成しますか&#x200B;]**という_ の**[!UICONTROL  メール」をクリックします。_セクション。
1. _テンプレートを選択_ ビューで、_チャネル_ フィルターを **[!UICONTROL メール]** に切り替えます。
1. _フィルター_ の横にある検索オプションを使用して、特定のメールテンプレートを検索します。
1. メールテンプレートをクリックして選択するか、複数のメールテンプレートを切り替えて「**[!UICONTROL 使用]**」をクリックします。 複数のテンプレートを選択した場合、バリアントの生成時に、選択したすべてのテンプレートが使用されてオプションが提供されます。

   コンテンツ作成の中心となるキャンバスが表示されます。

## パラメーターを追加

ガイドラインパラメーターを追加すると、コンテンツ生成プロセスが強化され、メールエクスペリエンスを生成するための不可欠な準備手順となります。

**パラメーターとアセットを追加するには**:

1. _パラメーター_ アイコンをクリックしてパラメーターオプションを展開し、参照パラメーターとアセットを追加します。
1. 「_パラメーター_」セクションで、ガイドライン（ブランド、ペルソナ、製品）を選択して、コンテンツの作成を通知します。

   これらのメニューから利用できるブランド、ペルソナ、製品がない場合は、[GenStudioにガイドラインを追加 ](/help/user-guide/guidelines/add-guidelines.md) します。

1. 「_コンテンツ_」セクションで、エクスペリエンスで使用するコンテンツ *および* を追加して、コンテンツの生成に影響を与えます。 アセットを追加する方法は 3 つあります。
   * **[!UICONTROL コンテンツから選択]** をクリックして、既に [!DNL Content] に公開されているアセット（画像またはビデオ）を選択します。 フィルターを使用して、検索結果をさらに絞り込みます。
   * **[!UICONTROL アップロード]** をクリックしてファイルを参照し、使用するアセットを選択します。 デバイスの参照に加えて、Microsoft OneDrive またはDropboxから読み込むこともできます。
   * アセットを「_コンテンツ_ セクションにドラッグ&amp;ドロップします。

   GenStudio コンテンツからアセットを選択する場合は、[[!DNL Content]](/help/user-guide/content/overview.md) に既に保存されているアセットから選択することになります。 チャネル、製品、言語などでフィルタリングすると、必要なアセットをすばやく見つけることができます。

パラメーターの追加が完了したら、「*パラメーター*」アイコンを再度クリックすると、「_パラメーター*」セクションと「*コンテンツ_」セクションを折りたたむことができます。

## プロンプトを使用

ガイドラインを選択したら、自然言語を使用してプロンプトを作成し、新しいメールエクスペリエンスのコンテンツの生成を開始します。

プロンプトの書き込みについて詳しくは、[ 効果的なプロンプトの書き込み ](/help/user-guide/effective-prompts.md) を参照してください。

**プロンプトを使用するには**:

1. _生成するエクスペリエンスを記述」_ プロンプトボックスにプロンプトを入力します。
   <!-- If the prompt box is not visible, click **[!UICONTROL Open to prompt]** to expand it. -->

<!-- 1. Optionally, click one of the prompt suggestions visible just above the prompt text box. Clicking a suggestion auto-fills the suggested prompt in the prompt box. -->
1. **[!UICONTROL 生成]** をクリックします。

デフォルトでは、生成された 4 つのバリエーション（追加したプロンプト、ガイドラインおよびコンテンツによってすべて強化）がキャンバスに表示されます。

## 生成されたメールを修正

承認または公開用に送信する内容を選択する前に [!DNL Content] メールフラグメントを編集したり、生成された一連のメールからバリアントを削除したりできます。

**生成されたバリアントを修正するには**:

* **メールを手動で編集するには**、メールフラグメント（件名行、ヘッダー、本文コピーなど）をダブルクリックし、必要に応じて編集します。

  件名行とプリヘッダーは、編集に 1 回のクリックのみが必要ですが、ヘッダー、本文コピー、コールトゥアクションでは、ダブルクリックが必要です。

* **メールを削除するには**、をクリックしてメールのタイトル（「メール 1/4」など）を選択し、「**[!UICONTROL バリアントを削除]**」をクリックします。

## ブランドの整合性の確認

生成されるメールを最適化し、ブランドアイデンティティに厳密に準拠するには、[_ブランドガイドラインチェック_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) の機能を活用します。この機能は、バリアントのブランド調整の概要を提供し、[_ブランド検証パネル_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) は、包括的なブランド検証の詳細を表示し、改善点を明らかにします。

個々のメールフラグメントを手動で編集するか、初期結果の [ 絞り込んだバリアントを生成 ](/help/user-guide/create/generate-variants.md) して、ブランドとの整合性を確保できます。

**ブランドの整合性を検証するには**:

1. バリアントの [**[!UICONTROL [!DNL Brand] guidelines check]**](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) アイコンをクリックすると、ブランドに対してチェックされたときのそのバリアントのパフォーマンスの概要が表示されます。
1. 改善が必要なフラグメントとガイドラインの詳細を取得するには、**[!UICONTROL 確認]**_をクリックするか_ 上部のメニューバーにあるブランド検証アイコンをクリックして [_ブランド検証パネル_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) を開きます。

1. 各メールを切り替えて、生成されたコンテンツを改善してブランドに合わせるようにする方法を確認します。
1. [ メールを手動で修正 ](#revise-generated-emails) または [ バリアントを生成 ](/help/user-guide/create/generate-variants.md) して、メールがブランドと密接に連携していることを確認します。

[ ブランド検証 ](/help/user-guide/guidelines/brand-validation.md) を参照してください。

## レビューと承認の取得

キャンバスの上部のメニューバーからアクセスできる承認パネルを使用して、レビューを取得、レビューコメントを追跡、関係者からの承認を取得します。

**レビューと承認を取得するには**:

1. [ ドラフトのメールエクスペリエンスの承認 ](/help/user-guide/approvals/request-review.md) を依頼する [ 承認リクエストの開始 ](/help/user-guide/approvals/approve-content.md)。
1. レビュープロセス中に [ レビュー担当者を削除または追加 ](/help/user-guide/approvals/review-and-edit.md#manage-approvals) できます。
1. [ レビュー用にコンテンツにアクセス ](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) し、修正要求を表示します。
1. レビューコメントごとにドラフトを編集し、[ メールエクスペリエンスを公開する ](#publish-and-export-experience) ようにします。

詳しくは、[ レビューと承認 ](/help/user-guide/approvals/overview.md) を参照してください。

## Publishと書き出しの経験

生成されたメールを現在および将来の使用で使用できるようにするには、メールを [!UICONTROL  コンテンツ ] に公開し、マーケティングキャンペーンで使用するために書き出します。

1. **新しいメールエクスペリエンスを公開するには**、上部のツールバーの **[!UICONTROL Publish]** をクリックします。
1. **新しいメールエクスペリエンスを書き出すには**、上部のツールバーにある **[!UICONTROL 書き出し]** をクリックします。
   1. CSV 形式と画像またはHTML形式のみを選択し、「**[!UICONTROL 書き出し]**」をクリックします。

詳細は、[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) を参照してください。
