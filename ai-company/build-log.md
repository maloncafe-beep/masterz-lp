# Build Log

## 2026-07-23

- 作成理由: 既存LPの構成を活かし、塾・理科講義の内容から「AIカンパニー」のAI活用支援LPへ転換するため。
- 作成物:
  - `brief.md`: AIカンパニーの事業内容、対象者、CTA、未確定事項を整理。
  - `copy.md`: ファーストビュー、問題提起、支援内容、メンバー紹介、FAQ、最終CTAのコピーを作成。
  - `index.html`: スマホ優先の静的LP。相談CTAは `mailto:zodiacm369@gmail.com`、副CTAは `https://maloncafe.shop/` へ接続。
  - `screenshots/`: 検証スクリーンショット保存先。
- 制作方式: HTMLテキスト中心。旧LPのteal基調とセクション構成を踏襲し、背景はCSSグラデーションで再構成。
- 確定情報:
  - 事業内容: AI活用支援で業務改革を並走。
  - 代表: マスターZ。
  - 社員: あい、ことは、りさ、はっく、さとる。
  - 問い合わせ: `mailto:zodiacm369@gmail.com`。
  - コーポレートサイト: `https://maloncafe.shop/`。
- 未設定:
  - 料金、契約期間、具体的な支援範囲、実績、お客様の声、導入事例。
- 検証予定:
  - 390px / 430pxで横スクロールが出ないこと。
  - PCで最大430pxのLPキャンバスが中央表示されること。
  - mailto、コーポレートサイト、メニューモーダル、Escでの閉じる動作が確認できること。
  - 個人の絶対パスやトークンがHTML内に残っていないこと。

## Verification

- 390px表示: `bodyScrollWidth=390`, `docScrollWidth=390`, 横スクロールなし。
- 430px表示: `bodyScrollWidth=430`, `docScrollWidth=430`, 横スクロールなし。
- PC表示: 1280px幅でLPキャンバス幅430px、中央表示OK。
- リンク: `mailto:zodiacm369@gmail.com` を5件、`https://maloncafe.shop/` を3件検出。
- モーダル: メニューボタンの開閉、Escでの閉じる動作OK。
- スクリーンショット:
  - `screenshots/mobile-390.png`
  - `screenshots/mobile-430.png`
  - `screenshots/desktop-1280.png`
- 旧塾LP文言確認: `RIKA`, `BESQUE`, `理科`, `講義`, `中学`, `受験`, `無料見放題` はAIカンパニー版HTMLから未検出。
- 絶対パス・トークン混入確認: `index.html` に個人絶対パス、APIキー、トークン類は未検出。
