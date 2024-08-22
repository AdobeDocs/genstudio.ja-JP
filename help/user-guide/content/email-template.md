---
title: パフォーマンスマーケター向けのAdobe GenStudio用メールテンプレートの準備
description: パフォーマンスマーケター向けにAdobe GenStudio用のカスタムメールテンプレートを作成する方法について説明します。
level: Intermediate
feature: Templates, Content
source-git-commit: 5bbc089fa7441ad8ce4cd84dd92889d1a22c0f61
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# パフォーマンスマーケター向けのAdobe GenStudio用メールテンプレートの準備

通常、デザイナーは、Adobe XDなどのデザインプログラムでテンプレートのビジュアルデザインを作成します。 メールテンプレートを設計、コーディング、テストしたら、アップロード用に準備し、パフォーマンスマーケターがGenStudioで使用できるようにします。

[ テンプレートの詳細 ](/help/user-guide/content/use-templates.md#anatomy-of-a-template) を参照してください。

## ガイドラインの追加

メタ広告テンプレートを準備する前に、パフォーマンスマーケター向けGenStudioに [ ガイドライン ](/help/user-guide/guidelines/overview.md) が追加され、関連するブランドの包括的な情報が入力されていることを確認します。 [ ブランドガイドライン ](/help/user-guide/guidelines/brands.md) は、生成されるコンテンツに直接影響します。

**例**：メールテンプレートの本文を 500 文字以下にする場合は、「本文」フィールドの [ チャネルガイドライン ](/help/user-guide/guidelines/brands.md#channel-guidelines) にその要件を追加します。

パフォーマンスマーケター向けにGenStudioにガイドラインが追加されていない場合は、デフォルトが使用されます。

## メールテンプレートのコーディング

テンプレートは、デザイン後、HTMLとインライン CSS を使用してコーディングされます。 コードは、様々なデバイスに対してクリーンでレスポンシブである必要があります。

[ テンプレートの例 ](/help/user-guide/content/customize-template.md#template-examples) を参照してください。

## メールテンプレートのテスト

メール配信またはプルーフプラットフォームを使用して、メールをテストし、様々なメールクライアントやデバイスで正しくレンダリングされていることを確認します。

メールテンプレートが次の条件を満たしていることをテストで確認します。

* レイアウトは、CSS メディアクエリを使用して様々な画面サイズに合わせて調整します
* ボタンをクリックして目的の場所に移動できます
* メールテンプレートは読みやすく、モバイルデバイスでも使用できます

## 生成されたコンテンツ領域の定義

パフォーマンスマーケター向けに、GenStudioのコンテンツを動的に入力するメールテンプレートの領域を定義します。

生成されたコンテンツ領域を定義するには：

* パフォーマンスマーケター向けGenStudioで自動生成するテンプレート内のテキスト要素（ヘッドライン、CTAなど）を特定します。
* Handlebars 構文を使用してプレースホルダーを挿入し、HTMLテンプレートを調整します。

[ コンテンツのプレースホルダー ](/help/user-guide/content/customize-template.md#content-placeholders) を参照してください。

## テンプレートのプレビュー

組み込みヘルパーを使用して、特定のコンテンツ領域の表示を制御します。 例えば、クリーンなプレビューリンクを維持しながら、書き出されたテンプレート内のリンクにトラッキングパラメーターを含めることができます。

[ テンプレートプレビュー ](/help/user-guide/content/customize-template.md#template-preview) を参照してください。

## テンプレートのアップロードと使用

テンプレートの設計、コーディング、テストおよびプレビューが完了したら、GenStudioにアップロードすると、パフォーマンスマーケターが新しいマーケティングコンテンツの生成に使用できます。

[ テンプレートの操作 ](use-templates.md) を参照してください。
