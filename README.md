# SS

サクマの各種サイト・プレゼント企画ページをまとめて管理するリポジトリです。
フォルダ構成がそのまま公開URLのパスになります（GitHub Pages）。

## フォルダ構成

```
SS/
├── main/
│   ├── sakumaschool/        スクール本体のサイト
│   │   ├── index.html       トップページ
│   │   ├── login.html       ログイン
│   │   ├── lesson.html      レッスン
│   │   ├── chapter.html     章
│   │   └── admin.html       管理画面
│   └── sakuma-sns-taizen/   SNS大全
│       ├── index.html
│       └── admin.html
└── present/                 プレゼント用ページ
    ├── sakuma-daihon-ai/    台本AI
    │   ├── index.html
    │   └── assets/
    └── sales-adventure/     セールスアドベンチャー
        └── index.html
```

> `main` はブランチ名ではなく、リポジトリ内のフォルダ名です。

## 公開URL

ベースURL: `https://infokksakuma-ops.github.io/SS/`

| ページ | URL |
| --- | --- |
| スクール | `.../SS/main/sakumaschool/` |
| SNS大全 | `.../SS/main/sakuma-sns-taizen/` |
| 台本AI（プレゼント） | `.../SS/present/sakuma-daihon-ai/` |
| セールスアドベンチャー（プレゼント） | `.../SS/present/sales-adventure/` |

※ 正確なベースURLは **Settings → Pages** で確認してください。

## ページを追加・更新する手順

1. 追加したいフォルダ（中に `index.html`）を用意する
2. GitHubで置きたい階層（例: `present/`）を開く
3. **Add file → Upload files** を選び、**フォルダごと**ドラッグ＆ドロップする
4. コミットメッセージを入れて **Commit changes**
5. 数分後、`.../SS/<階層>/<フォルダ名>/` で表示を確認する

## 注意点

- フォルダを開いて `index.html` だけをアップロードすると、意図しない階層に置かれてしまう。必ずフォルダごとアップロードする
- 画像やCSSなど別ファイルを読み込むページは、それらも一緒にアップロードする
- HTML内のリンクは `login.html` や `./login.html` のような相対パスにする（`/login.html` のように先頭が `/` だと、サブフォルダ配下では動かない）
- リポジトリがPublicの場合、中身は誰でも見られる。パスワードや社内情報は置かない
