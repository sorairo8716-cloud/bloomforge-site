# bloomforge.jp

Bloomforge Group公式Webサイト。GitHub Pagesでホスティングし、`bloomforge.jp`ドメインを
紐づけて公開する。2026-08-12、CEO指示「bloomforge.jpのSSL復旧およびBloomforge Group公式
サイトへの刷新」により、個人開発の屋号ページからBloomforge Group公式サイトへ刷新した。

現在の内容：
- `/` — Bloomforge Groupのトップページ（Hero / What We Do / Products / Experiments / Links）
- `/support` — Florafolioのサポートページ（変更なし、維持）
- `/privacy` — Florafolioのプライバシーポリシー（変更なし、維持）
- `/assets/` — Bloomforge Group公式ロゴ（`shared/brand/`と同一素材のWeb最適化版）

デザイン方針・掲載可否の判断根拠は`ceo-office`リポジトリの
`business-development-office/x-account-launch-proposal-2026-08-12.md`および
関連decisionsを参照。

## SSL証明書について（2026-08-12）

以前、GitHub Pages側のカスタムドメイン証明書が発行されないままの状態（`https_enforced: false`）
が続き、ブラウザでセキュリティ警告が出る不具合があった。原因はDNS設定ではなく（A/AAAA/CAAは
すべて正常だったことを確認済み）、GitHub側の証明書発行プロセスが完了しないまま止まっていた
こと。カスタムドメイン設定を一度解除→再設定することで証明書発行を再トリガーし解消した。
DNS（MX/SPF/DKIM等、Google Workspaceメール関連レコードを含む）は一切変更していない。

## 状態

2026-08-12時点：Bloomforge Group公式サイトとして刷新・公開済み。


## Corporate Website化（2026-08-12）

CEO指示「Bloomforge Group公式サイト再設計 — Corporate Website化」により、AI運営手法を
前面に出す表現を削除し、Mission/Vision/Products/Approach/Companyを中心とした一般的な
Corporate Website構成へ再設計した。GitHubへの主要導線（Header/Hero/Products内）は削除。
詳細・ベンチマーク根拠は`ceo-office`リポジトリの
`business-development-office/corporate-website-redesign-2026-08-12.md`参照。


## MVV正式決定の反映（2026-08-12）

CEO決定によりBloomforge Groupの正式Mission/Vision/Valuesを反映した。正本は
`ceo-office`リポジトリの`shared/bloomforge-group.md`「Mission / Vision / Values（正式版）」。
Our Approachセクションは正式Values（短縮形）へ置き換えた。


## Visual全面リデザイン（2026-08-12 第2回）

CEO指示「Bloomforge Group Corporate Website ビジュアル全面リデザイン」対応。情報設計・
正式MVVは維持したまま、Visual Design/Brand Experienceを全面刷新した。

- ロゴを透過PNGへ差し替え（白背景バグ修正）
- Design System刷新：Bloom Coral/Petal Pink/Sage Green/Bloom Ivory/Forge Brown/
  Warm Goldに役割分担を持たせたCSS変数を新設
- Hero：ボタニカルモチーフ（茎・葉・花・炎の粒子）を新規SVGで制作、Visual Heroへ刷新
- Products：Product個別のSVGアイコン付きVisualカードへ（実在しないスクリーンショットは
  不使用）
- Values：4項目それぞれに専用アイコン（手描きSVG）を追加
- Company：ボタニカル装飾アクセント付きのCardへ
- Contact：Bloom Coral系のCTAバンドへ
- Footer：4カラム構成へ整理
- Florafolioの表記を「Florafolio（フローラフォリオ）」へ修正、実仕様（seed-release-definition.md）と照合した説明文に更新
- `/support`・`/privacy`のヘッダー/フッターを新デザインへ統一（法的文言・Q&A本文は無変更、diff確認済み）
- Accessibility：コントラスト比WCAG AA未達箇所（brown-soft・coral系リンク・Contact
  バンド）を再調整して解消。Mission/Companyセクションにsr-only h2を追加し見出し構造を修正
