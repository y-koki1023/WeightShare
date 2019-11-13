# WeightShare

## 要件定義

### 背景

世の中にとは大抵監視されることに対しストレスを感じる。  
この特性をダイエットに活かす事はできないだろうか?  
活動をSNSに投稿 -> 周囲からの監視 ->  活動を途中で止める ->  周囲にバレる -> SNS報告する事は避けられない  -> 継続して活動を行うきっかけになる -> ダイエット成功  

活動を実行する事で、承認欲求を満たすことができるかもしれない

Q&A

- じゃあどんな内容をSNSに投稿すればいいんだろう  
  - アプリでテンプレートを用意  
- わざわざSNSに投稿するのが面倒臭い
  - アプリ内で必要な情報を入力すると自動でSNSにその情報を投稿
- わざわざアプリを使うメリットは?
  - SNS投稿の手間を緩和
  - 記録として残しやすい (Log)

### ターゲットユーザー

- SNSを頻繁に利用している
- ダイエットがしたいけど続かない
- 承認欲求を満たしたい  
and more...

### 使用されると思われるプラットフォーム

- スマートフォン (iOS and Android) 
- PC

スマートフォンで使用されるケースが高い

### 使用するべきアプリ形態

- 選択肢1
  - モバイル向けアプリ開発
    ユーザーが一番馴染みやすい形態(スマホユーザーが多いと考えられるため)  
    活動情報の登録自体にネットワーク環境が必要ない(ただしSNS投稿は不可)   
    サーバーサイドをこちらで用意する必要はない  
- 選択肢2
  - Webアプリ
    複数のプラットフォームに対応  
    個人的な学習コストはモバイルアプリに比べて少ない
    PWAでモバイル向けアプリとして対策ができる  

今回は学習コストの麺を考えて選択肢2(Webアプリでの開発を行う)

### 使用されるであろう技術

- フロント
  - React (Next.js)
  - Redux
  - Redux thunk
  - JavaScript
  - Html, css
- サーバーサイド
  - ~~Ruby on Rails~~
  - Elixer?
  - MySQL
  - oAuth and OpenID connect (Twitter)
- インフラ
  - nginx?

今回デザイン用にサードパーティライブラリを使用しない
