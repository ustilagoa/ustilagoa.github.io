# ustilagoa.github.io

iPhone / iPad 向けアプリのサポートページとプライバシーポリシー。
GitHub Pages（Jekyll）で `https://ustilagoa.github.io/` に公開している。

## 構成

- `_layouts/default.html` — 全ページ共通の見た目
- `_includes/` — 複数アプリで共通の文章。ここを直せば全ページに反映される
  - `no-tracking.md` — 広告・解析・トラッキングを行わない旨
  - `contact.md` — 問い合わせ先
  - `developer.md` — 開発者について
- `<アプリ名>/index.md` — サポートページ
- `<アプリ名>/privacy.md` — プライバシーポリシー

## アプリを追加するとき

1. フォルダを1つ作る
2. `index.md` と `privacy.md` を置く（`permalink` を忘れずに）。
   `index.md` の front matter に `appstore:` を書けば、`{{ page.appstore }}` で
   App Store リンクを置ける（ボタンの見た目は `.cta`）
3. `index.md`（トップ）の一覧に1行足す

共通の文章は `{% include contact.md %}` のように差し込む。同じ文章を2箇所に書かない。

連絡先メールアドレスは `_config.yml` の `email` に書き、`{{ site.email }}` で引く。
レイアウトからも include からもページ本文からも、同じ書き方で参照できる。

## App Store Connect に入れるURL

| アプリ | 用途 | URL |
|---|---|---|
| 鍵蔵 | サポートURL | https://ustilagoa.github.io/kagizo/ |
| 鍵蔵 | プライバシーポリシーURL | https://ustilagoa.github.io/kagizo/privacy/ |
| 青葉 | サポートURL | https://ustilagoa.github.io/aoba/ |
| 青葉 | プライバシーポリシーURL | https://ustilagoa.github.io/aoba/privacy/ |

## 注意

このリポジトリのコミットには `26980374+ustilagoa@users.noreply.github.com` を使う設定にしてある（`git config user.email`）。
個人のメールアドレスを公開履歴に残さないため。クローンし直したら設定し直すこと。
