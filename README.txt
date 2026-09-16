額田まつり 公式サイト（本番公開用）
=====================================

■ フォルダ構成
  index.html          … サイト本体（1ファイル完結）
  assets/
    poster-2026.jpg  … 2026年 ポスター
    venue-map-2026.jpg … 2026年 会場案内図
    poster-2025.pdf   … 2025年 ポスター（ダウンロード用）
    flyer-2025.pdf    … 2025年 チラシ（会場案内図入り・ダウンロード用）
    ogp.jpg           … SNSシェア時のサムネイル画像（1200×630）

  ※ index.html はこの assets フォルダを参照します。
    2つを同じ階層に置いたまま公開してください。


■ 公開方法A：Netlify Drop（いちばん簡単・無料）
  1) https://app.netlify.com/drop を開く（要ログイン／無料登録）
  2) この「prototype」フォルダごと、画面にドラッグ＆ドロップ
  3) 数秒で https://〇〇〇.netlify.app のURLが発行されます
  4) サイト設定から独自ドメインの割り当ても可能

■ 公開方法B：Cloudflare Pages（無料・高速）
  1) Cloudflare にログイン → Workers & Pages → Create → Pages
  2) 「Upload assets」でこのフォルダをアップロード（またはGit連携）
  3) デプロイ完了で https://〇〇〇.pages.dev のURLが発行されます


■ 公開後にやること（SNSシェアを綺麗に出すため）
  index.html の <head> 内、下記2行の
  「REPLACE-WITH-YOUR-DOMAIN」を、実際の公開URLに書き換えて再アップロード：
    <meta property="og:url"   content="https://REPLACE-WITH-YOUR-DOMAIN/">
    <meta property="og:image" content="https://REPLACE-WITH-YOUR-DOMAIN/assets/ogp.jpg">


■ 中身の更新について
  ・開催日／スケジュール／お知らせ … index.html 内のテキストを直接編集
  ・つくりもんの本写真が用意できたら、記録ギャラリーに差し替え
  ・「つくりもん単体」の写真は現状ありません（当日公開の演出として運用中）

■ 公開前チェック（正式サイトとして出す場合）
  ・地域（額田区・実行委員会）としての公開可否・運営主体の確認
  ・写真の掲載許可（撮影者・被写体）
  ・2026年の個別行事時刻が発表されたらスケジュールへ反映
  ・つくりもんの正式な地区数・地区名の確認

  出典・参考：2026年 額田まつりポスター・会場案内図、
              2025年 額田まつり公式ポスター・チラシ（森の京都）、
              額田のダシ行事（Wikipedia）
