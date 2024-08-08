---
title: GenStudio用のメールテンプレートの準備
description: GenStudioのカスタムメールテンプレートを作成する方法について説明します。
level: Intermediate
feature: Templates, Content
source-git-commit: 31f02218e02b1400ca9f32472acdecae03dbd304
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---


# GenStudio用メールテンプレートの準備

通常、デザイナーは、Adobe XDなどのデザインプログラムでテンプレートのビジュアルデザインを作成します。 メールテンプレートを設計、コーディング、テストしたら、GenStudioでアップロードおよび使用できるように準備できます。

[ テンプレートの詳細 ](/help/user-guide/content/use-templates.md#anatomy-of-a-template) を参照してください。

## ガイドラインの追加

メタ広告テンプレートを準備する前に、GenStudioに [ ガイドライン ](/help/user-guide/guidelines/overview.md) が追加され、関連するブランドの包括的な情報が入力されていることを確認します。 [ ブランドガイドライン ](/help/user-guide/guidelines/brands.md) は、生成されるコンテンツに直接影響します。

**例**：メールテンプレートの本文を 500 文字以下にする場合は、「本文」フィールドの [ チャネルガイドライン ](/help/user-guide/guidelines/brands.md#channel-guidelines) にその要件を追加します。

ガイドラインがGenStudioに追加されていない場合は、デフォルトが使用されます。

## メールテンプレートのコーディング

テンプレートは、デザイン後、HTMLとインライン CSS を使用してコーディングされます。 コードは、様々なデバイスに対してクリーンでレスポンシブである必要があります。

[ テンプレートの例 ](/help/user-guide/content/customize-template.md#template-examples) を参照してください。

## メールテンプレートのテスト

メール配信またはプルーフプラットフォームを使用して、メールをテストし、様々なメールクライアントやデバイスで正しくレンダリングされていることを確認します。

メールテンプレートが次の条件を満たしていることを確認するテスト：

* レイアウトは、CSS メディアクエリを使用して様々な画面サイズに合わせて調整します
* ボタンをクリックして目的の場所に移動できます
* メールテンプレートは読みやすく、モバイルデバイスでも使用できます

## 生成されたコンテンツ領域の定義

GenStudioのコンテンツを動的に入力するメールテンプレート内の領域を定義します。

生成されたコンテンツ領域を定義するには：

* GenStudioで自動生成するテンプレート内のテキスト要素（ヘッドラインやCTAなど）を指定します。
* Handblebars 構文を使用してプレースホルダーを挿入し、HTMLテンプレートを調整します。

[ コンテンツのプレースホルダー ](/help/user-guide/content/customize-template.md#content-placeholders) を参照してください。

## テンプレートのプレビュー

組み込みヘルパーを利用して、特定のコンテンツ領域の表示を制御します。 例えば、クリーンなプレビューリンクを維持しながら、書き出されたテンプレート内のリンクにトラッキングパラメーターを含めることができます。

[ テンプレートプレビュー ](/help/user-guide/content/customize-template.md#template-preview) を参照してください。

## テンプレートのアップロードと使用

テンプレートの設計、コーディング、テストおよびプレビューが完了したら、GenStudioにアップロードして、まったく新しいマーケティングコンテンツの生成に使用できます。

[ テンプレートの操作 ](use-templates.md) を参照してください。