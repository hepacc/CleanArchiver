# Monterey, Appleシリコン(M1)/arm64 対応版 CleanArchiver
Sparkle.framework を submodule 化して組み込み、ビルドしやすくした。

## 開発, 確認環境
- MacBook Pro (2021, M1) + Monterey
- MacBook Pro (2018, Intel) + Monterey

## ビルド
```
$ git clone --recursive https://github.com/hepacc/CleanArchiver.git
$ cd CleanArchiver
$ xcodebuild -configuration Release [-arch x86_64/arm64] build
```
ビルドに成功すると `CleanArchiver/build/Release` 以下に `CleanArchiver.app` ができる。
`-arch` 以下を省略すると x86_64/arm64 のユニバーサルバイナリ２ができる。
`-arch` を指定する場合は自分の環境に合わせて指定する。

<br>
<br>
以下、fork 元の README.md

---
---
---
<br>
<br>

# CleanArchiver

CleanArchiver is a simple and nifty archiving utility.

It creates **clean** gzip, bzip2, zip and compressed Disk Image archives
that don't include annoying files such as .DS_Store, Icon\r and .\_\*.


## Requirements

* Command Line Tools (Xcode)
