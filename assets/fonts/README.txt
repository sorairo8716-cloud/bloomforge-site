Bloomforge Group 公式サイトのフォント（自前ホスト）

このフォルダのフォントは、SIL Open Font License, Version 1.1（SIL OFL 1.1）で許諾された書体を、当サイトで使う文字に絞って（サブセット）配信しているものです。
各書体のライセンス文と著作権表示は、同じフォルダの OFL-*.txt と、各 woff2 ファイル内の著作権・ライセンスの記載にそのまま残しています。

書体と著作権表示
- Cormorant Garamond ……… Copyright 2015 The Cormorant Project Authors (github.com/CatharsisFonts/Cormorant)   [OFL-CormorantGaramond.txt]
- Noto Serif JP ……………… (c) 2017-2024 Adobe (http://www.adobe.com/)。許諾文書の表記は Copyright 2012 Google Inc.   [OFL-NotoSerifJP.txt]
- Noto Sans JP ……………… (c) 2014-2021 Adobe (http://www.adobe.com/), with Reserved Font Name 'Source'   [OFL-NotoSansJP.txt]
  （'Source' はAdobeの予約フォント名の表記で、当サイトのフォント名には使っていません。フォント名は Noto Sans JP のままです。）

加工の内容（OFL 1.1 の「改変版」に当たるため明記）
- 元ファイル：google/fonts リポジトリ（https://github.com/google/fonts）の ofl/ 配下の可変フォント。取得時点のコミット 2fe1e8c6b137fb13041a7cfca6fdcd8a910ea4dc（2026-11-03）。
  CormorantGaramond[wght].ttf sha256=b20b7d9626dd956b2c5e558692ad328b1f19e3275e2782db4fa07670d83f35e0
  CormorantGaramond-Italic[wght].ttf sha256=0f48ea6abb2084537854f7174c470991a463b13036309e3b50a81511611c530d
  NotoSerifJP[wght].ttf sha256=2fd527ba12b6a44ec30d796d633360da0aeba6c5d4af1304ce12bb4dc15a7dfc
  NotoSansJP[wght].ttf sha256=c2f3b4d463500a2ddcd3849cded1fceeb9fd6d1c32e6cbecd568453ba50fc68f
- 加工：①使う太さの範囲に絞る（Cormorant Garamond 400–700、同斜体は500、Noto Serif JP 500–700、Noto Sans JP 400–700）②当サイトで使う文字と基本の文字（英数記号・かな・句読点・全角記号）に絞る（サブセット）③woff2形式に圧縮。書体の絵柄（グリフの形）は変えていません。
- 作成スクリプト：CEO Office の it-operations/scripts/build_site_fonts.py（サイトの文言を足したときは、再実行して新しい文字を含めます）。

フォント単体の販売はしていません。
