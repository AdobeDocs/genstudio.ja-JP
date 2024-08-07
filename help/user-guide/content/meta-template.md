---
title: GenStudio用のメタ広告テンプレートの準備
description: GenStudioのカスタムメタ広告テンプレートを作成する方法について説明します。
level: Intermediate
feature: Templates, Content
source-git-commit: 6870f1b7056219d03cabbcc4e5ddbfa436b1a56d
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---


# GenStudio用のメタ広告テンプレートの準備

メタ広告テンプレートを作成するには、ソーシャルメディア用にカスタマイズされた構造化アプローチが必要です。 メタ広告テンプレートを設計およびテストしたら、GenStudioでアップロードおよび使用できるように準備できます。

## ガイドラインの追加

メタ広告テンプレートを準備する前に、GenStudioに [ ガイドライン ](/help/user-guide/guidelines/overview.md) が追加され、関連するブランドの包括的な情報が入力されていることを確認します。 [ ブランドガイドライン ](/help/user-guide/guidelines/brands.md) は、生成されるコンテンツに直接影響します。

**例**：メタ広告テンプレートの本文を 500 文字以下にする場合は、「本文」フィールドの [ チャネルガイドライン ](/help/user-guide/guidelines/brands.md#channel-guidelines) にその要件を追加します。

ガイドラインがGenStudioに追加されない場合は、デフォルトが使用されます。

## テンプレートのデザイン

通常、デザイナーは、Adobe XDなどのデザインプログラムでテンプレートのビジュアルデザインを作成します。

[ テンプレートの詳細 ](/help/user-guide/content/use-templates.md#anatomy-of-a-template) および [ テンプレート例 ](/help/user-guide/content/customize-template.md#template-examples) を参照してください。

### 広告仕様

GenStudioでは、メタ広告に対して次の縦横比をサポートしています。

* 正方形（1:1）: 1080 x 1080 ピクセル
* 縦長（4:5）: 1080 x 1350 ピクセル
* ストーリー（9:16）: 1080 x 1920 ピクセル

これらの縦横比のいずれかで広告が設計されていない場合、GenStudioは画像を適切なサイズに自動的に切り抜きます。

## メタ広告テンプレートのテスト

Meta の Creative Hub を使用してテンプレートをテストし、フィードやストーリーなどの様々なプレースメントで広告がどのように表示されるかを確認します。

メール配信またはプルーフプラットフォームを使用して、メールをテストし、様々なメールクライアントやデバイスで正しくレンダリングされていることを確認します。

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
