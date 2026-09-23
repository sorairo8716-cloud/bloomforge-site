# CLAUDE.md

このリポジトリは Bloomforge Group の公開サイト（`bloomforge.jp`）。静的HTML、GitHub Pages配信。

## CEO Office（全AI会社共通ルール）

作業開始時に `~/Developer/ceo-office/README.md` を読み、そこに書かれた全社共通ルール
（承認境界・秘密情報の扱い・外部公開文章の制作フロー等）を本リポジトリでも適用すること。
特に、このサイトの文言を書く・直すときは
[standards/external-copy-flow.md](~/Developer/ceo-office/standards/external-copy-flow.md)
（R-G-26、ChatGPTが本文を執筆しClaude Codeは目的・事実・仕様・導線を確認する）に従う。
会社固有の内容が本ファイル以下にある場合は、そちらを優先する。
（2026-09-23、全社ルール監査フォローアップにより新設。このリポジトリだけ本ファイルが
存在せず、R-G-26の対象であることが実装側から分からない状態だったため）

## 現状

- 個人情報を収集するフォーム・解析タグは無い（`mailto:`リンクのみ）。
- 自動デプロイ（GitHub Actions等）は無く、`main`へのpushがGitHub Pagesの配信対象になる。
