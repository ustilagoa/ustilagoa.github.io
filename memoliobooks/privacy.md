---
layout: default
title: プライバシーポリシー（メモリオ書籍）
permalink: /memoliobooks/privacy/
description: メモリオ書籍（MemolioBooks）のプライバシーポリシー
---

最終更新日: 2026年11月3日

「メモリオ書籍」（MemolioBooks。以下「本アプリ」）は、個人が開発・提供する iPhone / iPad 向けの読書記録アプリです。本ポリシーは、本アプリにおける情報の取り扱いについて説明します。

## 1. 収集する情報

ありません。氏名・メールアドレス・位置情報などの個人情報を収集しません。アカウント登録もありません。

開発者は、利用者が本アプリに何を記録したかを知る手段を持ちません。

## 2. 保存される情報

本アプリが保存するのは、利用者が登録した読書記録です。

| 情報 | 内容 |
|---|---|
| 書誌情報 | タイトル、著者、出版社、出版日、ISBN |
| 読書の記録 | 読了日、評価（★1〜5）、感想 |
| 書影の参照先 | 画像の URL（画像そのものは保存しません） |

保存先は、**利用者の端末と、利用者本人の iCloud** です。iCloud に入る場合もプライベートデータベースに保存され、**開発者が参照することはできません。** 同じ Apple アカウントでサインインした iPhone と iPad の間で記録を同期するために使います。

iCloud にサインインしていない場合、記録は端末内にとどまります。

## 3. 外部との通信

本アプリが外部に送信するのは、**ISBN だけ**です。

| 送信先 | 送るもの | 目的 |
|---|---|---|
| openBD（`api.openbd.jp`） | ISBN | タイトル・著者・出版社・出版日の取得 |
| Google Books（`books.google.com`） | ISBN | 書影の有無と画像 URL の取得 |

書影は、Google が返した URL から画像として読み込みます。

**読了日・評価・感想は、いかなる宛先にも送信しません。** アプリ内の検索（タイトル・著者）も端末の中だけで行っており、入力した語が外部に出ることはありません。

書影の画像を本アプリが保存することはなく、iOS の標準的な通信キャッシュに任せています。そのため、通信できない場所では書影が表示されないことがあります。

## 4. カメラ

バーコードから ISBN を読み取るためにカメラを使います。

- 読み取りは **端末内で** 行います（iOS の VisionKit）
- 読み取る対象は、書籍のバーコード（EAN-13）の数値だけです
- **撮影した画像は保存も送信もしません。** 画像を取り出す処理そのものを実装していません
- カメラを使わず、ISBN を手入力して登録することもできます

## 5. 広告・トラッキング・第三者への提供

{% include no-tracking.md %}

本アプリには広告 SDK、解析 SDK、その他の第三者製の実行時ライブラリを一切組み込んでいません。

## 6. データの削除

記録は、詳細画面から1件ずつ削除できます。削除は確認を挟みます。

まとめて削除することもできます。アプリの「設定」にある**「すべての記録を削除」**から、保存されている記録をすべて消せます。何件消えるかを示した確認を挟みます。iCloud で同期している場合は、**ほかの端末からも消えます。**

**本アプリを端末から削除しても、iCloud に同期された記録は iCloud 上に残ります。** これは iOS の仕組みによるもので、アプリ側から消すことはできません。完全に削除する場合は、iOS の「設定」から iCloud の保存容量を管理する画面を開き、本アプリのデータを削除してください。

## 7. 出典について

書誌情報は openBD、書影は Google Books から取得しています。本アプリは個人が開発したものであり、これらの提供元からの公認・関与を受けたものではありません。書影を表示している画面には、Google の定める帰属表示を併記しています。

## 8. お子様の利用について

本アプリは年齢を問わず情報を収集しません。お子様が利用した場合も同様です。

## 9. 本ポリシーの変更

本ポリシーの内容は、法令の変更や本アプリの機能追加に応じて改訂することがあります。変更する場合は、このページを更新し、最終更新日を改めます。収集する情報が増えるような変更を行う場合は、アプリの更新時に説明します。

## 10. お問い合わせ

{% include contact.md %}

---

## Privacy Policy (MemolioBooks)

Last updated: November 3, 2026

MemolioBooks ("the App") is a reading-log app for iPhone and iPad, developed and provided by an individual developer. This policy explains how the App handles information.

### 1. Information We Collect

None. The App does not collect personal information such as your name, email address, or location. There is no account registration.

The developer has no means of knowing what you record in the App.

### 2. Information That Is Stored

The App stores the reading records you enter: bibliographic details (title, author, publisher, publication date, ISBN), your reading record (finish date, rating, notes), and the URL of the cover image (not the image itself).

This is stored on your device and in your own iCloud account. When stored in iCloud, it is kept in your private database, which **the developer cannot access**. iCloud is used only to sync your records between an iPhone and iPad signed in to the same Apple Account. If you are not signed in to iCloud, your records stay on the device.

### 3. Network Communication

The only thing the App sends outside your device is an **ISBN**.

- openBD (`api.openbd.jp`) — an ISBN, to retrieve the title, author, publisher, and publication date
- Google Books (`books.google.com`) — an ISBN, to find out whether a cover image exists and to obtain its URL

The cover image is then loaded from the URL that Google returns.

**Your finish dates, ratings, and notes are never transmitted anywhere.** Search within the App (by title and author) runs entirely on your device; the words you type are not sent anywhere.

The App does not store cover images itself and relies on the standard iOS network cache. Cover images may therefore not appear when you are offline.

### 4. Camera

The App uses the camera to read an ISBN from a barcode.

- Recognition happens **on your device**, using VisionKit.
- Only the digits of a book barcode (EAN-13) are read.
- **Captured images are neither stored nor transmitted.** The App implements no path to extract an image at all.
- You can also enter an ISBN by hand instead of using the camera.

### 5. Advertising, Tracking, and Analytics

The App does not display ads, use analytics, or perform any third-party tracking. It does not request App Tracking Transparency (ATT) permission. The App does not share or sell any personal information to third parties (as none is collected). No advertising SDK, analytics SDK, or other third-party runtime library is included.

### 6. Deleting Your Data

Records can be deleted one at a time from the detail screen, with a confirmation step.

You can also delete everything at once from the App's Settings screen ("すべての記録を削除"). The confirmation states how many records will be removed. If iCloud sync is on, they are removed from your other devices as well.

**Deleting the App from your device does not remove records that were synced to iCloud.** This follows from how iOS works and cannot be changed by the App. To remove them, open the Settings app, go to the screen for managing iCloud storage, and delete the App's data there.

### 7. Data Sources

Bibliographic data comes from openBD, and cover images from Google Books. The App is developed independently and is not officially affiliated with or endorsed by either provider. Screens that display a cover image carry the attribution required by Google.

### 8. Children

The App collects no information from users of any age, including children.

### 9. Changes to This Policy

This policy may be revised to reflect legal requirements or new App features. The "Last updated" date above will be updated for material changes.

### 10. Contact

- Developer: ustilagoa
- [Contact form]({{ site.contact_form }})
