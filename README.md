# Emoji Lab

文字や手元の画像に動きと質感を付け、透明背景のPNGまたはアニメーションGIFとして書き出せるブラウザアプリです。

## 主な機能

- 文字入力、改行、字間、配置、太さの調整
- 28種類の動きと8種類の重ねがけ可能な質感
- 単色、グラデーション、虹色、縁取り、影
- PNG・JPEG・WebP・GIF画像の読み込み（GIFは静止画として使用）
- WOFF2・WOFF・TTF・OTFフォントの追加とブラウザ内保存
- 透明PNG、ループGIFの書き出し

サーバー処理やアップロードはありません。読み込んだ画像と追加フォントはブラウザ内で処理されます。

## GitHub Pages

静的ファイルだけで動作します。Repository settings の **Pages** で、`main` ブランチのルートを公開元に指定してください。

## 内蔵フォントとライセンス

次のフォントは、Google Fonts公式リポジトリのコミット `5fb648bb932bf1cdcd5fd71a73b79097e8666c36` で配布されているファイルをWeb配信用のWOFF2形式へ変換し、必要な書体だけ取得できるよう分割して同梱しています。いずれも **SIL Open Font License 1.1** です。各フォントの原文ライセンスは `fonts/licenses/` に収録しています。

| フォント | デザイナー | 配布元 |
| --- | --- | --- |
| Rampart One | Fontworks Inc. | `google/fonts` の `ofl/rampartone` |
| Rock 3D | Shibuya Font | `google/fonts` の `ofl/rock3d` |
| Potta One | Font Zone 108 | `google/fonts` の `ofl/pottaone` |
| New Tegomin | Kousuke Nagai | `google/fonts` の `ofl/newtegomin` |
| Yuji Boku | Kinuta Font Factory | `google/fonts` の `ofl/yujiboku` |

フォントファイルの著作権は各作者に帰属します。再配布や改変については、それぞれのOFL文書を確認してください。

## ファイル構成

- `index.html` — 画面
- `style.css` — デザイン
- `app.js` — 描画、アニメーション、書き出し
- `fonts/` — 内蔵フォント
