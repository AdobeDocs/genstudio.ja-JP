---
title: アセットとエクスペリエンスの管理
description: デジタルマーケティングジャーニーでの使用と再利用のために、ブランド承認済みアセットの管理を簡素化および強化します。
feature: Content, Assets, Experiences
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
source-git-commit: bd3c5c9ff12c962d4123ac992fb74cd94e184172
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 0%

---

# アセットとエクスペリエンスの管理

Adobe GenStudio for Performance Marketing [!DNL Content] は、デジタルマーケティングジャーニーでの使用と再利用のために、ブランド承認済みアセットの管理を簡素化および強化します。

## Assets美術館

[!UICONTROL Assets] ギャラリーには、承認されたアセットのインベントリが表示されます。 テーブルの左側の上にあるフィルター（ファネル）アイコンをクリックすると、**[!UICONTROL フィルター]** メニューが開き、多数のカテゴリから選択して、ギャラリーに表示されるアセットをフィルタリングできます。 検索（虫眼鏡）アイコンをクリックし、キーワードを使用してアセットを検索します。

以下は、[!UICONTROL Assets] ギャラリーの用語 `dog` に対する検索を示しています。

![ 犬で検索したAssets ビュー ](../../assets/content-assets.png)

### Assets場所

デフォルトでは、[!DNL Create] プロセスまたはアップロードを通じて [!DNL Content] に追加したアセットは、`GenStudio assets` リポジトリに保存されます。 `GenStudio assets` リポジトリは、GenStudio for Performance Marketingの読み取り/書き込みリポジトリです。 つまり、`GenStudio assets` リポジトリ内のアセットを保存、編集、削除できます。

右側のギャラリーの上にある **[!UICONTROL 場所]** リストを使用すると、接続されたAdobe Experience Manager（AEM）の [!DNL Assets Content Hub] リポジトリから選択できます。 AEM リポジトリを選択すると、そのリポジトリのアセットのインベントリがギャラリーに表示され、承認されたアセットをコンテンツ作成用の入力として活用できます。 フィルターオプションは、[!DNL AEM Assets Content Hub] で設定されたカテゴリを反映して変更されます。

AEM リポジトリーは読み取り専用です。つまり、ドラフト、新しいアセットまたはメタデータをAEM リポジトリーに保存することはできません。 アセット、エクスペリエンスおよびテンプレートのすべてのドラフトと最終更新は、新しい [ システムメタデータ ](asset-details.md#system-metadata) とともに `GenStudio assets` リポジトリに保存されます。

[AEM リポジトリをGenStudio for Performance Marketingに追加する方法については、[!DNL AEM Assets Content Hub] リポジトリの接続 ](connect-aem-repo.md) を参照してください。

## Assets管理

[!UICONTROL &#x200B; コンテンツ &#x200B;] では、パフォーマンスマーケターはデジタルアセットを簡単に保存、取得および管理できます。 `GenStudio assets` リポジトリーとAEM リポジトリーの両方を活用することで、アセットが適切に整理され、様々なマーケティングキャンペーンからアクセスできるようになります。 このマルチリポジトリアプローチは、環境全体でのアセットの使用を柔軟に制御し、承認された最新のアセットのみをマーケティング活動で使用できるようにします。

### アセットの追加

アセットを [!DNL Content] に追加すると、デフォルトでは、`GenStudio assets` リポジトリに保存されます。 「_[!UICONTROL アセットを追加]_」ボタンは、「_[!UICONTROL 場所]_ が `GenStudio assets` リポジトリの場合にのみ使用できます。

![Location フィールド ](../../assets/content-location.png){width="350" align="center"}

**1 つ以上のアセットを追加するには**:

1. _[!DNL Content]_&#x200B;で、「**[!UICONTROL アセットを追加]**」をクリックします。

1. _承認済みアセットを追加_ 表示で、ファイルをドロップスペースにドロップします。 オプションで、**[!UICONTROL 参照]** を使用してローカルファイルから選択したり、DropboxまたはMicrosoft OneDrive からファイルを読み込んだりできます。

1. 「_詳細を追加_」セクションで、**[!UICONTROL キャンペーン名]** を選択するか、新しい名前を入力します。

1. 検出性を向上させるには、「**詳細**」セクションに _ブランド名_、_ペルソナ_、_地域_、_キーワード_ などのオプションの詳細を追加します。

   提供する情報が多いほど、GenStudio for Performance Marketingの堅牢な機能を体験できます。 リストから 1 つ以上の詳細を選択するか、必要に応じて新しい詳細（キーワードを使用するなど）を入力します。 追加した各詳細は、リストの下に表示されます。 詳細を削除するには、「**`x`**」をクリックします。

   追加した詳細は、このアクションで追加されたすべてのアセットに適用されます。

   [ メタデータの詳細 ](/help/user-guide/content/asset-details.md#system-metadata) を参照してください。

1. **[!UICONTROL アセットを追加]** をクリックします。

1. アセットのアップロードが完了したら、「**完了**」をクリックします。

1. アップロードした新しいアセットを表示するには、キャンバスの下部にある _使用可能な新しいアセット_ 通知で **[!UICONTROL 更新]** をクリックします。

<!-- 
In the future, need guidance on template upload errors. For now, the UI just says error.
-->

### コンテンツを検索

このフィルターと検索のインターフェイスは迅速かつレスポンシブで、生産的な検索ファーストのエクスペリエンスを提供します。 各 [!DNL Content] 表示には、理想的なアセット、エクスペリエンスまたはテンプレートを絞り込むためのフィルターオプションが表示されます。 アセットとエクスペリエンスの場合は、キャンペーンと特定のガイドライン（特定の製品に対して作成されたコンテンツなど）を選択できます。

[ キーワード ](asset-details.md#user-defined-metadata) および [ 属性 ](/help/user-guide/insights/attributes.md) に基づいて検索結果を絞り込むフィルターがあります。 例えば、キャンペーンの新しいエクスペリエンスを構築するのに役立つ、特定のファイルタイプや件名のアセットを検索することができます。

_エクスペリエンス_ を検索する場合、**[!UICONTROL 作成者]** フィルターを使用して、自分または特定のユーザーが作成したエクスペリエンスのみを表示するようにリストを制限できます。

**再利用するコンテンツを検索するには**:

1. _[!DNL Content]_&#x200B;で、「**[!UICONTROL Assets]**」セクションを選択します。

1. **[!UICONTROL 場所]** リストからアセットリポジトリを選択するか、正しいアセットリポジトリを表示していることを確認します。 デフォルトのリポジトリは `GenStudio assets` です。

   >[!IMPORTANT]
   >
   >_場所_ リストを使用できるのは [AEM リポジトリに接続 ](connect-aem-repo.md) している場合のみです。

1. **[!UICONTROL 検索]** （虫眼鏡）をクリックして、キーワードまたは説明を入力します。

1. _[!UICONTROL フィルター]_ リストからカテゴリを選択して、検索を絞り込みます。 例えば、PNG ファイルを検索する場合は、「**[!UICONTROL ファイル形式]**」をクリックし、「**PNG**」を選択します。

   検索を絞り込めば絞り込むほど、使用できるフィルターオプションが少なくなります。 すべてのフィルターを削除するには、「**[!UICONTROL すべてクリア]**」をクリックします。

1. 全体表示および詳細リスト用のアセットを選択します。

   **[!UICONTROL ダウンロード]** （下矢印）をクリックして、ローカルワークステーションでアセットを使用します。
