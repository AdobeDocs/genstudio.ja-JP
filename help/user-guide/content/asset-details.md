---
title: アセットの詳細
description: パフォーマンスのAdobe GenStudioマーケターは、検索性とパフォーマンストラッキングのために、豊富なメタデータを含む承認済みコンテンツを保存します。
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: 95eb7c2eaeeceedf3abe5ab16e1e7c2de7bf8117
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 1%

---

# アセットの詳細

パフォーマンスのAdobe GenStudioマーケターは、検索性とパフォーマンストラッキングのために、リッチなメタデータを含む承認済みコンテンツを保存します。

各アセット（エクスペリエンスとテンプレートを含む）には、コンテンツのパフォーマンスを識別、追跡、使用および学習するのに役立つ _詳細_ （メタデータ）が関連付けられています。

**アセットの詳細を表示するには**:

1. _[!DNL Content]_で、アセット、エクスペリエンスまたはテンプレートを選択します。 アセットをクリックすると、そのアセットのフォーカスされたビューが開きます。

1. アセット表示で、右側の _[!UICONTROL 詳細]_ セクションを確認します。

   >[!TIP]
   >
   >「_[!UICONTROL 詳細]_」セクションが表示されない場合は、「**[!UICONTROL 情報]** （i）」アイコンをクリックします。

アセットの詳細には、作成またはアップロード処理中に適用されたメタデータが含まれます。 アセットメタデータタイプには、[ システムメタデータ ](#system-metadata) および [ ユーザー定義メタデータ ](#user-defined-metadata) が含まれます。

>[!NOTE]
>
>AEM リポジトリからのAssetsには、異なるメタデータが表示されます。 AEM Assets Content Hub アセットの詳細を設定する方法については、[ アセットの表示の設定 ](connect-aem-repo.md#step-4-configure-asset-visibility) を参照してください。

## システムメタデータ

アセットのアップロード時に、一部のアセットメタデータが自動的に収集されます。 デフォルトのシステムメタデータは編集できません。

アセットに対して保存および取得されるデフォルトのメタデータには、ファイルの名前、寸法、ソースなどがあります。

### 生成されたタグ

承認済みアセットを [!DNL Content] に保存すると、GenStudio for Performance のマーケターは、Adobeの AI と機械学習機能を使用してアセットを調査し、アセットの機能に基づいてタグを適用します。 例えば、猫の写真では、`pet photography` や `cat` などのスマートタグや、写真の中で支配的な色を識別するカラータグが生成される場合があります。 タグは編集できません。

### 生成されたコンテンツメタデータ

新しいアセットやエクスペリエンスの生成に使用する情報は、使用されたプロンプトなどのメタデータになります。 コンテンツが承認されると、プロンプトは編集できませんが、新しいコンテンツを生成するための出発点として使用できます。

## ユーザー定義のメタデータ

ユーザー定義メタデータは、アセットのコンテンツにマーケティングコンテキストを追加するので、マーケターはアセットの使用方法とエンゲージメント方法を理解できます。

[ アセットをアップロード ](/help/user-guide/content/manage-assets.md#add-assets) する際に、パフォーマンスマーケター向けGenStudioにメタデータとして存在する一連のオプションのアセット詳細を定義できます。 さらに詳細を含めると、検索とフィルタリングでのアセットの識別が向上します。

### メタデータの詳細

次の表に、アセットの作成時に定義できるメタデータ（アセットの詳細）を示します。

| フィールド | 説明 |
| ------------- | ----------- |
| キャンペーン（プロジェクト名） | アセットと共にキャプチャおよび保存されるデフォルトのメタデータ |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) がパフォーマンスマーケター向けにGenStudioに追加され、使用するために公開されました |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) をパフォーマンスマーケター向けにGenStudioに追加して使用 |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) をパフォーマンスマーケター向けにGenStudioに追加して使用 |
| チャネル | GenStudio for Performance Marketers で使用するアセットのコンテンツタイプ（メール、メタ広告など） |
| 期間 | 四半期、シーズン、年など、使用したアセットの期間。 例：`Winter 2023` |
| 地域  | アセットが使用される地域。 例：`North America`, `APAC`, `Italy` |
| 言語 | アセットを使用する言語。 例：`Spanish` |
| キーワード | 資産の特性や目的の絞り込みに活用するキーワード |

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
