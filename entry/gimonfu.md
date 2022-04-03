---
title: はてなブログのコンテンツをgimonfuでいい感じに管理する
date: 2022-04-03T08:40:52.000Z
id: "13574176438079445233"
draft: false
---
本ブログを管理するのにgimonfuというツールを使っており、これがとても便利なので紹介します。

# この文章の目標

はてなブログをやっている人、始めたい人にgimonfuの良さを知ってもらうこと。

# ブログのコンテンツは手元のファイルで管理したい

> Markdownで管理できるから

これは、[はてなブログ、はじめました。 - ちくわのブログ](https://chikuwa111.hatenablog.com/entry/hello-hatenablog)で書いた、ブログのプラットフォームをはてなブログにした理由の1つです。

一長一短ではありますが、私が書くものはできるだけプレーンテキストで管理したいと考えています。そのため、日々のメモもMarkdownで残しています。[^1]

ブログのコンテンツもプレーンテキストで管理することで、移行のしやすさや執筆環境をローカルで自由に整えられる、といったメリットを享受できます。

その際大きな壁となるのがプレーンテキストの内容をブログにアップロードする作業です。ここを楽にしてくれるのが今回紹介するgimonfuです。

# gimonfu

[yammerjp/gimonfu: CLI to manage hatena-blog articles](https://github.com/yammerjp/gimonfu)

gimonfuについては[作者のQiita記事](https://qiita.com/yammerjp/items/1a38857f6bafb20f065d)で詳しく書かれているのでここでは省きます。簡単に紹介すると、GitHubのリポジトリにMarkdownファイルをpushすればはてなブログが更新される、という楽ちん環境を作るためのツール、となります。

最初は[blogsync](https://github.com/x-motemen/blogsync)で管理しようとしていました。しかしblogsyncはローカルのためのツールであり、blogsyncでデリバリー部分も仕組み化するのは難しそうだと心が折れかけていました。もしgimonfuと出会っていなかったら本ブログは生まれていなかったかもしれません、、

# 私の管理環境と今後の展望

[chikuwa111/chikuwa111.hatenablog.com](https://github.com/chikuwa111/chikuwa111.hatenablog.com)

これがコンテンツを管理しているリポジトリです。現状は、mainブランチにpushされたらgimonfuで同期をとる、という仕組みのみ入っています。

次にやりたいことは、プルリクエストを作ったらPrettierのフォーマットとTextlintのレビューが走る仕組みの導入です。ここら辺の環境がパワーアップしたらまたブログで紹介します。

# まとめ

[gimonfu](https://github.com/yammerjp/gimonfu)を使っていい感じにブログのコンテンツを管理しましょう！


[^1]: 参考：[vscode-memoを使っている - chikuwa111](https://scrapbox.io/chikuwa111/vscode-memo%E3%82%92%E4%BD%BF%E3%81%A3%E3%81%A6%E3%81%84%E3%82%8B)
