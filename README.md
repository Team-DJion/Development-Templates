# Development Templates（開発テンプレート置き場）

Team-DJion の汎用テンプレートを、特定のAIアプリに依存しない「URLで開ける形」で置く公開リポジトリ。
司令塔（Muse / Grok Bot 等）が変わっても、URLと中身はそのまま使える。

## 構造 — 1テンプレート＝1フォルダ

```
index.html                 テンプレート一覧（カタログ）
moodboard/index.html       ムードボード（形容詞起点・4ステップ）入力版 — P2-03
p1-01-problem-brief/       P1-01 アイデア・目的の整理
p1-02-user-problem/        P1-02 ユーザー・課題の理解
p1-03-market-research/     P1-03 市場・競合・トレンド調査
p1-04-award-benchmark/     P1-04 優秀作品・受賞基準の分析
p1-05-feasibility-risks/   P1-05 技術・費用・リスクの初期評価
p1-06-value-options/       P1-06 価値提案・差別化案
p1-07-gtm-hypothesis/      P1-07 初期マーケティング仮説
p1-08-success-metrics/     P1-08 成功指標・検証計画
p1-09-owner-decision/      P1-09 オーナー承認（方向性合意）
p2-02-ux-requirements/     P2-02 ユーザー体験・要求の設計
p2-04-concept-approval/    P2-04 コンセプト方向性の合意
p2-05-flow-design/         P2-05 情報設計とフロー・画面構成
p2-06-design-system/       P2-06 デザインシステム
p2-08-acceptance/          P2-08 受入条件とテスト設計
p2-09-design-approval/     P2-09 設計承認と実装範囲確定
p5-08-review-gate/         P5-08 レビューゲート判定
p6-08-evidence-gate/       P6-08 実機・品質ゲートの証拠集約
p7-06-release-approval/    P7-06 リリース承認（P7-03 セキュリティGo/No-Go 内包）
p9-07-improvement-agreement/ P9-07 改善方向のHTML合意
```

記入済みの実物の置き場: ここに置くのは空の「型」だけ。案件で入力した実物は、各開発案件のリポジトリに、その工程の成果物名（例：problem-brief、design-system、acceptance-and-tests）で保管する。ブラウザの自動保存は下書き用で、正本は書き出したHTML／JSONを案件リポジトリへ入れたものとする。

全テンプレート共通フレーム v1: ヘッダー（案件名／工程番号／担当AI／版／状態）＋欄の色分け（人が書く／AIが書く／決定）＋要点が先＋証拠リンクと未検証＋次工程への引き継ぎ＋ブラウザ内自動保存と書き出し（入力済みHTML／JSON）。

新しいテンプレートは、フォルダを1つ足して、一覧（index.html）にカードを1枚足すだけで増やせる。
各テンプレートのURLはフォルダ単位で固定される（例: `.../moodboard/`）。

## ルール

- 各テンプレートは単一HTMLファイルで完結させる（外部送信なし、入力はブラウザ内保存＋ファイル書き出し）。
- ここに置くのは汎用テンプレートのみ。案件ごとの入力内容や秘密情報は置かない。
- 様式の正本（決定済みデザイン）は private の Design-Library 側。本リポジトリは配布・利用のための公開置き場。
