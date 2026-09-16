# 額田まつり 案内サイト

京都府福知山市夜久野町額田の秋祭り「額田まつり（額田のダシ行事）」を紹介する非公式案内サイト。
静的サイト（HTML1ファイル＋画像内蔵）。ビルド不要でそのまま公開できます。

## 構成
```
index.html        サイト本体（1ファイル完結）
assets/
  poster-2026.jpg 2026年 ポスター
  venue-map-2026.jpg 2026年 会場案内図
  poster-2025.pdf 2025年 ポスター（DL用）
  flyer-2025.pdf  2025年 チラシ（会場案内図入り・DL用）
  ogp.jpg         SNSシェア用サムネイル（1200×630）
netlify.toml      公開設定（publish = ルート）
```

## 公開（Netlify + GitHub 連携）
1. このリポジトリを GitHub に push
2. Netlify → Add new site → **Import an existing project** → このリポジトリを選択
3. Build command：**空欄** ／ Publish directory：**`.`（ルート）**
4. 以降は push するたびに自動デプロイ

## 公開後の設定（SNSシェア画像）
`index.html` の `<head>` 内、`REPLACE-WITH-YOUR-DOMAIN` を実際の公開URLに書き換える：
```
<meta property="og:url"   content="https://（公開URL）/">
<meta property="og:image" content="https://（公開URL）/assets/ogp.jpg">
```

## 更新のしかた
- 開催日・スケジュール・お知らせ … `index.html` のテキストを直接編集
- つくりもんの写真は毎年の開催週に撮影 → `assets/` に追加し、記録ギャラリーに1行追加

## 出典・参考
2026年 額田まつりポスター・会場案内図／2025年 額田まつり公式ポスター・チラシ（森の京都）／額田のダシ行事（Wikipedia）
