---
title: アセットの詳細
description: GenStudioでは、検索性とパフォーマンストラッキングのために、リッチなメタデータを使用して承認済みコンテンツを格納します。
feature: Attributes, Assets
source-git-commit: c8fa0cf1633a5ca0ab94d9a0f33d9b7e7d6d61ed
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 7%

---


# アセットの詳細

GenStudioでは、検索性とパフォーマンストラッキングのために、リッチなメタデータを使用して承認済みコンテンツを格納します。

各アセット（エクスペリエンスとテンプレートを含む）には、コンテンツのパフォーマンスを識別、追跡、使用および学習するのに役立つ _詳細_ （メタデータ）が関連付けられています。

アセットメタデータタイプには、[ システムメタデータ ](#system-metadata) および [ ユーザー定義メタデータ ](#user-defined-metadata) が含まれます。

## システムメタデータ

アセットのアップロード時に、一部のアセットメタデータが自動的に収集されます。 デフォルトのシステムメタデータは編集できません。

アセットに対して保存および取得されるデフォルトのメタデータには、ファイルの名前、寸法、ソースなどがあります。

### 生成されたタグ

アセットが承認されて [!DNL Content] に保存されると、GenStudioはAdobeの AI および機械学習機能を使用して、カラーやトーンなどのアセットの機能や、アセットの機能を識別するキーワードに基づいてタグを生成します。 タグは編集できません。

### 生成されたコンテンツメタデータ

新しいアセットやエクスペリエンスの生成に使用する情報は、使用されたプロンプトなどのメタデータになります。 コンテンツが承認されると、プロンプトは編集できませんが、新しいコンテンツを生成するための出発点として使用できます。

## ユーザー定義のメタデータ

ユーザー定義メタデータは、アセットのコンテンツにマーケティングコンテキストを追加するので、マーケターはアセットの使用方法とエンゲージメント方法をより深く理解できます。

[ アセットをアップロード ](/help/user-guide/content/manage-assets.md#add-assets) する際に、GenStudioにメタデータとして存在する一連のオプションのアセット詳細を定義できます。

### メタデータの詳細

次の表は、アセットの作成時に定義できるメタデータ（アセットの詳細）の詳細を示しています。

| フィールド | 説明 | 編集可能 | 必須 |
| ------------- | ----------- | -------- | -------- |
| キャンペーン名（プロジェクト名） | アセットと共に取得され保存されるデフォルトのメタデータ | ○ | × |
| ブランド名 | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) がGenStudioに追加され、使用するために公開されました | ○ | × |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) がGenStudioに追加されて使用されるようになりました | ○ | × |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) がGenStudioに追加されて使用されるようになりました | ○ | × |
| チャネル | メールやメタ広告など、アセットが使用されるGenStudioのコンテンツタイプ | ○ | × |
| 期間 | 四半期、シーズン、年など、使用したアセットの期間。 例：`Winter 2023` | ○ | × |
| 地域  | アセットが使用される地域。 例：`North America`, `APAC`, `Italy` | ○ | × |
| 言語 | アセットを使用する言語。 例：`Spanish` | ○ | × |
| キーワード | アセットの目的を識別するために使用されるキーワード | ○ | × |

## アセットの詳細の表示

**アセットの詳細を表示するには**:

1. _[!DNL Content]_で、アセットを選択します。

1. アセット表示で、右側の _[!UICONTROL 詳細]_ セクションを確認します。

   「_[!UICONTROL 詳細]_」セクションが表示されない場合は、「**[!UICONTROL 情報]** （i）」アイコンをクリックします。

>[!TIP]
>
>アセットの詳細は [!DNL Insights] からも表示できます。 [!DNL Insights] は、エクスペリエンス全体にわたる使用状況の統計とパフォーマンスコンテキストを提供します。 _[!DNL Insights]_で、「**[!UICONTROL Assets]**」セクションを選択します。

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->