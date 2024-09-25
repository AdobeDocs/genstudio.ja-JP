---
title: バリアントの管理
description: 生成されるバリアントとアセットをカスタマイズし、デジタルマーケティングのニーズに合わせて強化します。
feature: Content, Assets, Experiences
source-git-commit: e99fadb7c440adbfa52759d6b392e08d0ee6d155
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---


# バリアントの管理

Performance Marketing [!DNL Create] のAdobe GenStudioを使用すると、生成されるバリアント（メール、メタ広告など）をカスタマイズおよび強化して、デジタルマーケティング戦略で使用できます。

[ エクスペリエンスの作成 ](/help/tutorials/tutorials.md) 時に、生成されたバリアントのコンテンツとアセットを個別にまたはバッチで変更できます。 個々のマイクロレベルでバリアントを管理する機能により、生成されたコンテンツの各部分を明示的に管理できます。

## ドラフト名を変更

生成されたバリアントドラフトには、キャンバスの上部にデフォルト名が表示されます。 デフォルトのドラフト名は、チャネルタイプ、日付、生成時刻を含む次の規則を使用します。

*例*:「Meta：名称未設定ドラフト - 09.5.24、午前 9:56」

**デフォルト名を変更するには**:

1. バリアントのセットを生成したら、キャンバスの上部にあるデフォルトの _名称未設定のドラフト_ 名をクリックします。
1. テキストを選択し、新しい名前を入力します。
1. テキストフィールドの外側をクリックして保存します。

## テキストを手動で編集

生成されたバリアントのテキストフィールドを編集できます。 様々なフレーズや言葉を試して、オーディエンスのテキストを絞り込みます。 例えば、バリアントのテキストを手動で改訂して、選択した画像でヘッドラインの外観をプレビューできます。

**生成されたバリアントのテキストを手動で編集するには**:

1. バリアントのセットを生成した後、バリアント内の編集可能なテキストをダブルクリックします。
1. 新しいテキストを入力します。
1. テキストフィールドの外側をクリックして保存します。

<!-- ## Re-generate sections

GenStudio for Performance Marketing has the built-in functionality to regenerate single sections of generated variants using _[!UICONTROL Suggested edits]_ and fresh prompts.

For example, you can re-generate the headline section of one Meta ad variant to see how it looks with a specific background asset using the _[!UICONTROL Suggested edits]_ options—_[!UICONTROL Rephrase]_, _[!UICONTROL Shorten]_, or _[!UICONTROL Lengthen]_—and entering a new prompt.

**To re-generate individual variant sections**:

1. After generating a set of variants, single-click editable text in a variant.
1. (_Optional_) Enter a new prompt to change the focus of the regenerated content.
1. Select a _[!UICONTROL Suggested edits]_ option—_[!UICONTROL Rephrase]_, _[!UICONTROL Shorten]_, or _[!UICONTROL Lengthen]_.
1. Click **[!UICONTROL Generate]**.
1. If you want to regenerate results, click the regenerate icon adjacent to _Results_.
1. From the _Results_ that appear, select the desired option and click **[!UICONTROL Replace]**.

   The variant is updated with the revised text.

## Crop assets

You can manually crop and reposition image assets in individual generated variants.

**To crop and reposition images in variants**:

1. After generating a set of variants, hover over an image within a variant.
1. Click **[!UICONTROL Apply Crop]**.
1. Zoom in and out and drag the image into the desired position.
1. Click **[!UICONTROL Apply]**.

   The cropped image is automatically saved and visible for the variant. -->

## アスペクト比の変更

目的の広告サイズに合わせて、メタ広告の縦横比をすばやく変更できます。

使用可能なサイズ/縦横比は次のとおりです。

* 1:1 平方（メタ）
* 縦 4:5 （メタ）
* 9:16 縦（Meta）
* 250 x 980 （ディスプレイ広告）

>[!NOTE]
>
>使用可能なテンプレートに応じて、他の縦横比やサイズも使用できます。

**生成されたメタ広告の縦横比を変更するには**:

1. バリアントのセットを生成したら、キャンバスの左側にある縦横比のサイズ変更アイコン（ボックスの隅を指す矢印）を選択します。

   広告に現在使用されている縦横比は、_[!UICONTROL サイズ変更]_ ウィンドウの上部に表示されます。

   このリビジョンの影響を受けるバリエーションの数は、ウィンドウの右上隅に示されています。 _例_:「4/4 のバリエーション」

1. 使用可能な縦横比を選択します。

   キャンバスに現在表示されていないアスペクト比のサイズのみ選択できます。

1. **[!UICONTROL 複製とサイズ変更]** をクリックします。

[!DNL Create] は、選択した新しい縦横比に基づいて各バリアントのコピーを作成します。 初期のアスペクト比を含むすべてのバリアントがキャンバスに存在します。

例えば、最初に 1:1 の縦横比で 4 つのバリアントを生成し、縦横比を 4:5 に変更した場合、合計 _8_ のバリアントがキャンバスで使用できるようになりました。

## バリアントを削除

保存や再利用を予定していない生成されたバリアントはすべて削除できます。

作業用キャンバスに、積極的にリファインまたは使用しているバリアントのみが表示されるように、不要なバリアントを削除します。

**生成されたバリアントを削除する手順は次のとおりです**。

1. バリアントのセットを生成したら、バリアントの上の名前をクリックします。

   バリアントがハイライト表示され、ショートカットメニューが表示されます。

1. 使用可能なメニューオプションから **[!UICONTROL 削除]** を選択します。

   バリアントが削除されます。

## バリアントごとのブランド検証

_[!UICONTROL ブランドガイドラインのチェック]_ および _[!UICONTROL ブランド検証パネル]_ を使用して、一貫性のあるブランドアイデンティティとバリアントの整合性を維持します。

[ ブランド検証 ](/help/user-guide/guidelines/brand-validation.md#improve-brand-alignment) を参照してください。
