WUWA COMMUNITY Discord Server紹介サイト — 更新版

■ 今回の変更
- 日本語 / English の言語切り替えを維持・拡張
- script.js の日本語サイト文言を英語版にも反映
- ABOUT THE COMMUNITY のタイトル・説明・4コンテンツを指定内容に更新
- ABOUT のサブテキストを拡大
- JP / EN COMMUNITY のテキスト領域を拡大し、指定した <br> を維持
- JP / EN COMMUNITY の「コミュニティに参加する」リンクを削除
- CHANNEL GUIDE を01〜06のインタラクティブなチャンネル紹介に変更
- チャンネルは左側、紹介写真＋紹介文は右側に表示
- PCはカーソル操作、モバイルはタップ操作に対応
- GALLERY は最大20枚の画像を掲載でき、右→左へゆっくり無限ループ
- COMMUNITY EVENTS はタイトル→説明文の順に配置し、右側に写真を追加
- COMMUNITY EVENTS の参加ボタンを削除
- STAFF は管理者・副管理者の2名に変更

■ 最初に変更する場所
script.js の CONFIG を変更してください。
INVITE_URL = 実際のDiscord招待URL
SERVER_ID = DiscordサーバーID（人数表示を使う場合）

■ CHANNEL GUIDE の写真
script.js の CHANNELS に各チャンネルの背景画像を指定しています。
現在は既存の hero.jpg / hero2.jpg / hero3.jpg / hero2(2).jpg を使用しています。
実際のチャンネル写真に変更する場合は、CHANNELS の bg を変更してください。

■ GALLERY の写真
index.html の GALLERY 内に20枚分の画像スロットがあります。
各 <img src="..."> の src を実際の写真ファイルへ変更してください。
現在はサイトに同梱されている既存画像を仮配置しています。
20枚すべてを別画像にする必要はありません。掲載したい枚数に応じて src を差し替えてください。

■ STAFF
index.html の staffGrid 内の名前・役職を変更してください。

■ Cloudflare
GitHubリポジトリとCloudflare Workersを接続している場合、GitHubへ変更をpushするとCloudflare側で自動デプロイできます。

■ JavaScript
外部ライブラリのインストールは不要です。ブラウザだけで動作します。
