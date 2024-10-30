---
title: Adobe GenStudio for Performance Marketingのレビューと承認
description: GenStudio for Performance Marketingのレビューおよび承認プロセスについて説明します。
feature: Approval
exl-id: c83f47c0-e8ae-4c54-84b3-c50f67d6b3c2
source-git-commit: bd3c5c9ff12c962d4123ac992fb74cd94e184172
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Adobe GenStudio for Performance Marketingのレビューと承認

レビューと承認のワークフローにより、クリエイティブチームから法務エキスパートまでのすべての関係者が、生成される AI によって生成されるブランドアセットを含む、キャンペーンのアセットとエクスペリエンスを効率的にレビューおよび承認できるようになります。

## [!DNL Review and Approval] ワークフローの利点

* **堅牢で反復的な生成 AI コンテンツ作成のサポート**。 ブランドに合わせたコンテンツを組織内で作成およびデプロイするプロセスは、非常に反復的です。 GenStudio for Performance Marketingのジェネレーティブ AI 機能は、数百ものアセットバリアントをすばやく作成することをサポートしています。 各レビュー担当者は、アセットのドラフトを承認する前に、1 つのアセットに対して複数の変更をリクエストすることがあります。 レビュー担当者が多いほど、すべての関係者が最終的なバリアントに合意するまでの潜在的なイテレーションの数が多くなります。

* **クリエイティブの整合性のサポート**。 承認は、コンテンツ作成者を承認プロセスに引き続き関与させることで、ブランドアセットのクリエイティブの整合性を保護します。 レビューと承認のプロセスにクリエイティブの関係者（コンテンツ作成者やクリエイティブディレクターなど）を関与させることで、最終的な出力がビジョンやブランドアイデンティティに合致していることを確認できます。

* **Campaign の目標と法的要件の遵守** 承認プロセスは、コンテンツがキャンペーンの目標をサポートしていることを検証するのに役立ちます。 すべてのマーケティング資料が法的基準および規制基準に確実に準拠するようにすることで、リスクと潜在的な法的問題を最小限に抑えることができます。

## レビューと承認のライフサイクル

レビューと承認のワークフローの主なフェーズには、次のものが含まれます。

* [作成したコンテンツのレビューと承認をリクエストする](./request-review.md)
* [コンテンツのレビューと編集](./review-and-edit.md)
* [コンテンツを承認](./approve-content.md)
* [Publish コンテンツ](./publish-content.md)

## レビューをリクエストしたりコンテンツを承認したりできるのは誰ですか？

アセットまたはエクスペリエンスを作成した場合は、組織の承認チェーンの他のユーザーに、自分の作業について正式にレビューしコメントするよう依頼できます。 GenStudio for Performance Marketing組織のメンバーは誰でもドラフトをレビューできますが、ドラフトにコメントしたり、ドラフトを承認したりできるのは、指名された承認者のみです。

## [!DNL Content] 件のドラフトについて

_ドラフト_ は、レビューと承認プロセスを経ていない、アセットまたはエクスペリエンスの暫定的なバージョンです。 ドラフトステータスは、ドラフトがレビューおよび承認プロセスのどこに存在するかを識別します。 一意のドラフト ID は、各ドラフトを識別します。 ID は、ドラフトが承認されて [!DNL Content] に公開されるまで有効です。 ドラフトのレビューコメントと承認は、この個々のドラフト ID に関連付けられています。

ドラフトがレビューと承認プロセスを完了し、[!DNL Content] に公開されると、ドラフト ID は期限切れになり、GenStudio for Performance Marketingには関連するコメントと承認ステータスが保存されません。 ドラフト URL が無効になりました。

ドラフトステータスは、レビューと承認のプロセスを進めるときのコンテンツドラフトの状態を取得します。 レビュー中のアセットを作成したGenStudio for Performance Marketing コンテンツエディターに、ドラフトまたは承認に対して変更をリクエストすると通知されます。 承認者は下書きの状態を変更し、下書きをさらに修正する必要があるか、承認可能かを示します。 指定されたすべての承認者は、アセットまたはエクスペリエンスを公開する前に、そのアセットまたはエクスペリエンスを承認する必要があります。

使用可能なドラフトステータス：

**通知済み**：コンテンツエディターは、ドラフトをレビューする準備が整ったことを承認者に通知することで、レビューと承認のプロセスを開始しました。
**作業が必要**:1 人以上の承認者がコンテンツドラフトの変更をリクエストしたことを示します。 この状態のコンテンツは [!DNL Content] に保存できません。
**承認済み**：指定されたすべての承認者が、アセットまたはエクスペリエンスを承認しました。 コンテンツエディターで、アセットまたはエクスペリエンスにメタデータを追加して、[!DNL Content] に保存できるようになりました。

## 通知

GenStudio for Performance Marketingの製品内通知では、アセットのステータスの変更やコメントに応じて、承認者とコンテンツ編集者をリアルタイム `@mention` 更新します。 通知は、複数のレビュー、編集、承認のサイクルを通じた迅速な反復をサポートします。

コンテンツ編集者および承認者は新規登録して、これらの通知をSlackで受け取ることができます。 [Experience Cloudのサービスの購読 ](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences#slack) を参照してください。

承認参加者が実行するアクション製品内通知およびメール通知が自動でトリガーされます。 承認プロセスを開始すると、指定された承認者にメールと製品内通知の両方が届きます。 承認者がコメントを追加したり、決定を下したりするたびに、製品内およびメール通知 `@mention` 使用してループを維持できます。 通知には、コンテンツドラフトへのリンクが含まれます。

コンテンツのレビューと承認プロセスを開始すると、すべての承認とレビューコメントが通知されます。 ただし、承認者には、`@mention` が含まれるコメントのみが通知されます。