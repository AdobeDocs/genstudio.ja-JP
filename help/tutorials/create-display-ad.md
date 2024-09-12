---
title: ディスプレイとエクスペリエンスの作成
description: パフォーマンスマーケター向けに、Adobeでディスプレイ広告エクスペリ  [!DNL GenStudio]  ンスを作成する方法を説明します。
feature: Brands Service, Guidelines, Content Generation, Generative AI, Create, Experiences, Variant Generation
role: User
level: Beginner
type: Tutorial
recommendations: noDisplay
source-git-commit: 9624429977e21af614173c5078c6b470c8b5a147
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

# ディスプレイとエクスペリエンスの作成

このチュートリアルでは、GenStudio for Performance Marketers [[!DNL Create]](/help/user-guide/create/overview.md) （左側のナビゲーションエリアの絵筆アイコン）を使用してブランド化されたディスプレイ広告体験を生成する方法を実演します。

魅力的なディスプレイ広告体験をデザインするには、開始する前に [ パフォーマンスマーケター向けGenStudioにガイドラインを追加 ](/help/user-guide/guidelines/add-guidelines.md) し、[ プロンプトの記述の基本 ](/help/user-guide/effective-prompts.md) を詳しく調べることをお勧めします。

## テンプレートを選択

ディスプレイとエクスペリエンスを作成するには、使用可能なテンプレートを使用してコンテンツのフレームワークを提供します。

**ディスプレイ広告テンプレートを選択するには**:

1. _[!DNL Create]_**[!UICONTROL で、「今日は何を作成しますか？」の_ 広告を表示]** をクリックします。_セクション。
1. _フィルター_ の横にある検索オプションを使用して、特定のディスプレイ広告テンプレートを見つけます。
1. _テンプレートを選択_ ビューで、ディスプレイ広告テンプレートをクリックします。
1. **[!UICONTROL 使用]** をクリックします。

   コンテンツ作成の中央ハブとして機能するキャンバスが表示されます。

## パラメーターを追加

[ ガイドライン ](/help/user-guide/guidelines/overview.md) とアセットを _パラメーター_ のプロンプトエリアに追加すると、コンテンツ生成プロセスが過大評価され、メールエクスペリエンスを生成するための不可欠な準備手順となります。

**パラメーターとアセットを追加するには**:

1. _パラメーター_ アイコンをクリックして、プロンプト領域を展開します。
1. 「_パラメーター_」セクションで、ガイドライン（[!DNL Brands]、[!DNL Personas]、[!DNL Products]）を選択して、コンテンツの作成を通知します。

   これらのメニューに表示されるブランド、ペルソナまたは製品がない場合は、[ パフォーマンスマーケター向けGenStudioにガイドラインを追加 ](/help/user-guide/guidelines/add-guidelines.md) してください。

1. エクスペリエンスで使用するコンテンツを追加する場合は **[!UICONTROL コンテンツを選択]** をクリックし *コンテンツの生成に影響を与える場合は* および」をクリックします。
   * **[!UICONTROL コンテンツから選択]** をクリックして、[!DNL Content] に公開済みのアセット（画像）を選択します。 フィルターを使用して、検索結果をさらに絞り込みます。
   * **[!UICONTROL アップロード]** をクリックしてファイルを参照し、使用するアセットを選択します。 デバイスの参照に加えて、Microsoft OneDrive またはDropboxから読み込むこともできます。
   * アセットを「_コンテンツ_ セクションにドラッグ&amp;ドロップします。
1. **[!UICONTROL 使用]** をクリックします。

パラメーターの追加が完了したら、「_パラメーター_ アイコンをもう一度クリックして、プロンプト領域を折りたたみます。

## プロンプトを入力

ガイドラインを選択したら、自然言語を使用してプロンプトを作成し、新しいディスプレイとエクスペリエンスのコンテンツの生成を開始します。 生成されるディスプレイとエクスペリエンスの品質を高めるには、詳細で説明的なプロンプトを作成することが重要です。

プロンプトの書き込みについて詳しくは、[ 効果的なプロンプトの書き込み ](/help/user-guide/effective-prompts.md) を参照してください。

**プロンプトを入力するには**:

1. _生成するエクスペリエンスを記述」_ プロンプトボックスにプロンプトを入力します。
1. 「**[!UICONTROL 生成]**」をクリックします。

デフォルトでは、4 つのバリエーション（追加したプロンプト、ガイドラインおよびコンテンツによってすべて強化される）が生成され、キャンバスに表示されます。

## 生成されたディスプレイ広告を変更

に承認または公開するために送信する内容を選択する前に [!DNL Content] ディスプレイ広告セクションとテキストフィールドを編集したり、生成されたバリアントを削除したりできます。

**生成されたバリアントを修正するには**:

* **ディスプレイとドラフトの名前を [ 編集](/help/user-guide/create/manage-variants.md#change-draft-name)** するには、キャンバスの上部にある _名称未設定のドラフト_ タイトルをクリックし、新しいタイトルを入力します。
* **ディスプレイ広告を [ 手動で編集](/help/user-guide/create/manage-variants.md#manually-edit-text)** するには、ディスプレイ広告の任意のセクションまたはフィールド（件名行、ヘッダー、本文コピーなど）をダブルクリックし、必要に応じて編集します。
* **広告のサイズと縦横比を [ 変更](/help/user-guide/create/manage-variants.md#change-aspect-ratio)** するには、_[!UICONTROL サイズ変更]_ ボタン（キャンバスの左側にボタンアイコンが表示されたボックス）をクリックし、すべてのバリアントに適用する新しいサイズと縦横比を選択します。 バリアントが複製され、サイズが変更されます。

<!-- # Preview for device

When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.

**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## ブランドの整合性の確認

生成される広告を最適化し、ブランドアイデンティティに厳密に準拠するには、[_ブランドガイドラインチェック_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) の機能を活用して、バリアントのブランド調整の概要を提供し – [_ブランド検証パネル_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) は、包括的なブランド検証の詳細を表示し、改善点を明らかにします。

**ブランドの整合性を検証するには**:

1. バリアントの [**[!UICONTROL [!DNL Brand] guidelines check]**](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) アイコンをクリックすると、ブランドに対してチェックされたときのそのバリアントのパフォーマンスの概要が表示されます。
1. 改善が必要なフラグメントとガイドラインの詳細を取得するには、**[!UICONTROL 確認]**_をクリックするか_ 上部のメニューバーにあるブランド検証アイコンをクリックして [_ブランド検証パネル_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) を開きます。

1. 生成されたコンテンツを改善して、ブランドに合わせやすくする方法を確認します。
1. [ 手動で広告を改訂 ](#revise-generated-display-ads) し、メールがブランドと密接に連携するようにします。

[ ブランド検証 ](/help/user-guide/guidelines/brand-validation.md) を参照してください。

## レビューと承認の取得

キャンバスの上部のメニューバーからアクセスできる承認パネルを使用して、レビューを取得、レビューコメントを追跡、関係者からの承認を取得します。

**レビューと承認を取得するには**:

1. [ ドラフトのメールエクスペリエンスの承認 ](/help/user-guide/approvals/request-review.md) を依頼する [ 承認リクエストの開始 ](/help/user-guide/approvals/approve-content.md)。
1. レビュープロセス中に [ レビュー担当者を削除または追加 ](/help/user-guide/approvals/review-and-edit.md#manage-approvals) できます。
1. [ レビュー用にコンテンツにアクセス ](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) し、修正要求を表示します。
1. レビューコメントごとにドラフトを編集し、[ メールエクスペリエンスを公開する ](#publish-and-export-experience) ようにします。

[ レビューと承認 ](/help/user-guide/approvals/overview.md) を参照してください。

## Publishと書き出しの経験

生成したディスプレイ広告を現在および将来の使用で使用できるようにするには、[!UICONTROL  コンテンツ ] に公開し、マーケティングキャンペーンで使用するために書き出します。

1. **新しいディスプレイ広告エクスペリエンスを公開するには**、上部のツールバーの **[!UICONTROL Publish]** をクリックします。
1. **新しいディスプレイ広告エクスペリエンスを書き出すには**、上部のツールバーにある **[!UICONTROL 書き出し]** をクリックします。
   1. フォーマット（JPGと PNG のみ）を選択し、「**[!UICONTROL エクスポート]**」をクリックします。

詳しくは、[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) を参照してください。
