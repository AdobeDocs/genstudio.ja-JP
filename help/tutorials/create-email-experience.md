---
title: メールエクスペリエンスの作成
description: Adobeでメールエクスペリエンスを作成する方法を説明します  [!DNL GenStudio]。
feature: Content, Brands Service, Guidelines, Content Generation
role: User
level: Beginner
type: Tutorial
recommendations: noDisplay
source-git-commit: c8fa0cf1633a5ca0ab94d9a0f33d9b7e7d6d61ed
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---


# メールエクスペリエンスの作成

このチュートリアルでは、GenStudio [[!DNL Create]](/help/user-guide/create/overview.md) （左側のナビゲーションエリアの絵筆アイコン）を使用してブランドのメールエクスペリエンスを生成する方法を説明します。

効果的なメールエクスペリエンスを作成するには、開始する前に [GenStudioにガイドラインを追加 ](/help/user-guide/guidelines/add-guidelines.md) し、[ プロンプトの作成の基本 ](/help/user-guide/effective-prompts.md) をブラッシュアップすることをお勧めします。

## テンプレートを選択

新しいメールエクスペリエンスの作成を開始するには、使用可能なテンプレートを使用してコンテンツのフレームワークを提供します。

**メールテンプレートを選択するには**:

1. _[!DNL Create]_で、「今日は何を作成しますか&#x200B;]**という_ の**[!UICONTROL  メール」をクリックします。_セクション。
1. _フィルター_ の横にある検索オプションを使用して、特定のメールテンプレートを検索します。
1. クリックしてメールテンプレートを選択し、「**[!UICONTROL 使用]**」をクリックします。

   コンテンツ作成の中心となるキャンバスが表示されます。

## パラメーターを追加

[ ガイドライン ](/help/user-guide/guidelines/overview.md) とアセットを _パラメーター_ のプロンプトエリアに追加すると、コンテンツ生成プロセスが過大評価され、メールエクスペリエンスを生成するための不可欠な準備手順となります。

**パラメーターとアセットを追加するには**:

1. _パラメーター_ アイコンをクリックして、プロンプト領域を展開します。
1. 「_パラメーター_」セクションで、ガイドライン（[!DNL Brands]、[!DNL Personas]、[!DNL Products]）を選択して、コンテンツの作成を通知します。

   これらのメニューから利用できるブランド、ペルソナ、製品がない場合は、[GenStudioにガイドラインを追加 ](/help/user-guide/guidelines/add-guidelines.md) します。

1. 「**[!UICONTROL コンテンツを選択]**」をクリックして、エクスペリエンスで使用するコンテンツを追加 *および* をクリックすると、コンテンツの生成に影響が及びます。
   * **[!UICONTROL コンテンツから選択]** をクリックして、[!DNL Content] に公開済みのアセット（画像）を選択します。 フィルターを使用して、検索結果をさらに絞り込みます。
   * **[!UICONTROL アップロード]** をクリックしてファイルを参照し、使用するアセットを選択します。 デバイスの参照に加えて、Microsoft OneDrive またはDropboxから読み込むこともできます。
   * アセットを「_コンテンツ_ セクションにドラッグ&amp;ドロップします。

パラメーターの追加が完了したら、「_パラメーター_」アイコンを再度クリックすると、プロンプト領域を折りたたむことができます。

## プロンプトを入力

ガイドラインを選択したら、自然言語を使用してプロンプトを作成し、新しいメールエクスペリエンスのコンテンツの生成を開始します。 詳細なプロンプトは、曖昧なプロンプトや説明のつかないプロンプトよりも高品質の出力を生成します。

プロンプトの書き込みについて詳しくは、[ 効果的なプロンプトの書き込み ](/help/user-guide/effective-prompts.md) を参照してください。

**プロンプトを入力するには**:

1. _生成するエクスペリエンスを記述」_ プロンプトボックスにプロンプトを入力します。
1. **[!UICONTROL 生成]** をクリックします。

デフォルトでは、4 つのバリエーション（追加したプロンプト、ガイドラインおよびコンテンツによってすべて強化される）が生成され、キャンバスに表示されます。

## 生成されたメールを修正

承認または公開用に送信する内容を選択する前に [!DNL Content] メールフラグメントを編集したり、生成された一連のメールからバリアントを削除したりできます。

**生成されたバリアントを修正するには**:

* **メールのドラフト名を編集するには**、キャンバス上部の _名称未設定のドラフト_ タイトルをクリックし、新しいタイトルを入力します。
* **メールを手動で編集するには**、メールフラグメント（件名行、ヘッダー、本文コピーなど）をダブルクリックし、必要に応じて編集します。

  件名行とプリヘッダーは、編集に 1 回のクリックのみが必要ですが、ヘッダー、本文コピー、コールトゥアクションでは、ダブルクリックが必要です。

* **メールを削除するには**、をクリックしてメールのタイトル（「メール 1/4」など）を選択し、「**[!UICONTROL バリアントを削除]**」をクリックします。

## ブランドの整合性の確認

生成されるメールを最適化し、ブランドアイデンティティに厳密に準拠するには、[_ブランドガイドラインチェック_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) の機能を活用します。この機能は、バリアントのブランド調整の概要を提供し、[_ブランド検証パネル_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) は、包括的なブランド検証の詳細を表示し、改善点を明らかにします。

**ブランドの整合性を検証するには**:

1. バリアントの [**[!UICONTROL [!DNL Brand] guidelines check]**](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) アイコンをクリックすると、ブランドに対してチェックされたときのそのバリアントのパフォーマンスの概要が表示されます。
1. 改善が必要なフラグメントとガイドラインの詳細を取得するには、**[!UICONTROL 確認]**_をクリックするか_ 上部のメニューバーにあるブランド検証アイコンをクリックして [_ブランド検証パネル_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) を開きます。

1. 各メールを切り替えて、生成されたコンテンツを改善してブランドに合わせるようにする方法を確認します。
1. [ メールを手動で修正 ](#revise-generated-emails) し、メールがブランドと密接に連携するようにします。

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