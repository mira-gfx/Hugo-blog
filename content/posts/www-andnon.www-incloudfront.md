+++
draft = true
thumbnail = "images/CloudFlont+Route53.../thumbnail.png"
tags = ["CloudFront","aws"]
date = "2020-03-13T21:05:36+09:00"
lastmod = "2020-03-13T21:05:36+09:00"
title = "CloudFlont+Route53でwww.付きでも無しでもアクセスできるようにする"
description = ""
+++
こんにちは[@mira_tech](https://twitter.com/mira_tech)です。
[「ブログのリニューアルを成し遂げたぜ！」](https://www.saltandsugar.tech/posts/renewblog/)でも書いた様に改装前のブログにはURLに`www.`を付けないとアクセスできないというそこそこ致命的な問題(半月以上放置)があリました。ググっても`www.`ありから`www.`なしにリダイレクトする方法しか出てこず、手順もめんどくさそうだったのでしょうがなく適当にそれっぽいことしたらできたっていう話です。**自己責任で！お気をつけて！**

## 端的に
**二つ作っちゃえばいいんだよ！**
{{< img src="images/CloudFlont+Route53.../CloudFront-Management-screen.png" >}}

www.なしとwww.あり両方のディストリビューション作っちゃえばええんだよ(もちろん設定内容は同じにして)
### 注意
CIツールでブログのデプロイとか自動化してる時はきちんと追加したディストリビューションのキャッシュの消去のことも記述しないと`www.`ありだとアクセスできるデータが`www.`無しだとアクセスできないみたいなおかしいことが起こっちゃいますよ！

## 余談(上と全く関係ない)
解説しようとしたけど解説することなかったわ

**ブログ2日間連続で更新してます！(過去最高記録)** ほめて！！！！！！



