---
title: csTimer日本語版ユーザーズガイド(非公式)
excerpt: csTimerの機能および操作方法について解説します。
description: csTimer日本語版の非公式ユーザーズガイドです。主要な機能および操作方法について解説します。
date: 2020-05-24 17:00:00 +0900
header:
  teaser: /assets/img/cstimer/csTimerGuide.png
  og_image: /assets/img/cstimer/csTimerGuide.png
  image: /assets/img/cstimer/csTimerGuideHeader.png
categories:
  - cstimer
tags:
  - ユーザーズガイド
  - Tools
  - タイマー
layout: single
author_profile: true
sidebar: true
permalink: /cstimer/usersguide

toc: true
toc_label: "目次"
toc_icon: "align-left"
toc_sticky: true

gallery_ui:
  - url: /assets/img/cstimer/cstimer_menu.png
    image_path: /assets/img/cstimer/cstimer_menu.png
    alt: "メニュー"
    title: "メニュー"
  - url: /assets/img/cstimer/cstimer_statmenu.png
    image_path: /assets/img/cstimer/cstimer_statmenu.png
    alt: "統計情報"
    title: "統計情報"
  - url: /assets/img/cstimer/cstimer_solvedetail.png
    image_path: /assets/img/cstimer/cstimer_solvedetail.png
    alt: "ソルブ詳細"
    title: "ソルブ詳細"

gallery_sessions:
  - url: /assets/img/cstimer/cstimer_sessionmanager.png
    image_path: /assets/img/cstimer/cstimer_sessionmanager.png
    alt: "セッションマネージャー"
    title: "セッションマネージャー"
  - url: /assets/img/cstimer/cstimer_sessionmanager_op.png
    image_path: /assets/img/cstimer/cstimer_sessionmanager_op.png
    alt: "セッションマネージャー(操作)"
    title: "セッションマネージャー(操作)"

gallery_options:
  - url: /assets/img/cstimer/cstimer_options.png
    image_path: /assets/img/cstimer/cstimer_options.png
    alt: "オプション"
    title: "オプション"

gallery_tools:
  - url: /assets/img/cstimer/cstimer_tool_dist.png
    image_path: /assets/img/cstimer/cstimer_tool_dist.png
    alt: "分布"
    title: "分布"
  - url: /assets/img/cstimer/cstimer_tool_trend.png
    image_path: /assets/img/cstimer/cstimer_tool_trend.png
    alt: "トレンド"
    title: "トレンド"


---
本記事は書きはじめたばかりです！とりあえず雛形だけ作った状態なので、まだ内容はあまりありません(2020/05/24)
{: .notice--info}

## 本ユーザーズガイドについて {#about}
![](/assets/img/cstimer/cstimer_screenshot.png){:width="600px" height="auto" class="img-responsive align-center"}

本ユーザーズガイドは、**スピードキューブ用オンラインタイマーアプリ「csTimer」日本語版の機能をまとめて解説するためのものです。** 開発者に許諾を得たものではなく、日本語版UIに準拠して紹介をするものです。

csTimerは中国のスピードキューバー[Shuang Chen (cs0x7f)](https://www.speedsolving.com/wiki/index.php/Shuang_Chen)によって2012年にリリースされ、2020年05月現在もアクティブに機能追加や修正が進められています。スピードキューブの計測用のタイマーとして必要な基本的機能が揃っているだけでなく、他のタイマーアプリにないような機能も豊富にあります。それぞれの機能の概要や使い方についてまとめたものがなかったため、非公式にユーザーズガイドを執筆することにしました。[^1]

## 主要機能は？ {#features}
### スクランブル {#scramble}
**csTimerは全てのWCA公式種目のスクランブルに対応しています。** また、特定のサブステップを練習するためのスクランブルや、リレー競技(234リレーなど)、エッジのみ、コーナーのみ、簡単なクロス、など、非常に多くのスクランブルタイプを選択することができます。
#### 全てのWCA公式種目
- 3x3x3
- 2x2x2
- 4x4x4
- 5x5x5
- 6x6x6
- 7x7x7
- 3x3x3目隠し
- 3x3x3最少手数
- 3x3x3片手
- クロック
- メガミンクス
- ピラミンクス
- スキューブ
- スクエア1
- 4x4x4目隠し
- 5x5x5目隠し
- 3x3x3複数目隠し

#### 特定のサブステップを練習するためのスクランブル
- F2L
- OLL
- PLL
- ZBLL
その他多数

### 統計機能 {#stat}
Ao5やAo12などの基本的な統計機能のほか、セッション単位でのソルブ管理、区間タイムの計測機能（マルチフェイズ機能）などが含まれます。
### ソルバー {#solver}
クロス、X-Cross、2x2x2の一面、スキューブの一面、スクエア1の整形などのソルバー機能があります。クロスなど特定のステップの学習や練習に利用できます。
### バックアップ {#backup}
クラウドストレージ（csTimerサーバー、Google Driveなど）へのデータバックアップ機能があります。また、ローカルのエクスポート／インポート機能があります。

## 基本操作 {#basic-usage}
### UI {#user-interface}
{% include gallery id="gallery_ui" caption="ユーザーインターフェイス" %}

ユーザーインターフェイスの詳細について記載予定
{: .notice--danger}

### タイマーをスタート・ストップする {#timing}
スペース、インスペクションあり、タイピング、スタックタイマー連携

### セッション管理 {#session-management}
{% include gallery id="gallery_sessions" caption="セッションマネージャー" %}

**計測したデータは「セッション」という単位で保存することができます。**タイム一覧を表示しているエリアからセッションマネージャーを使うことができます。セッションごとに名前をつけて、スクランブルタイプ(3x3x3、4x4x4など)、統計情報(Ao5/Ao12/Ao100など)、フェイズ数(分割数)が管理できます。

#### セッションのマージ
次の手順で2つのセッションをマージすることができます。
1. セッションマネージャーから**他のセッションの最後にマージしたいセッションの名前**をクリックします。より新しいセッションが該当することが多いでしょう。
1. マージしたいセッションの右側にある**「...」**をクリックします。ドロップダウンメニューが表示されるので、**「マージ」**を選択します。より古いセッションが該当することが多いでしょう。
1. 確認画面が表示されるので「OK」を選択します。この操作はキャンセルすることができないため、マージしたい順序になっていることをよく確認しましょう。

![](/assets/img/cstimer/cstimer_session_merge.png){:width="600px" height="auto" class="img-responsive align-center img-thumbnail"}

#### セッションの分割
次の手順でセッションを分割することができます。
1. セッションマネージャーから**分割したいセッションの名前**をクリックします。
1. セッションの右側にある**「...」**をクリックし、分割を選択します。
1. ポップアップメニューが表示されるので、分割したいソルブ数を入力します。セッション内の最新のソルブから指定した数のソルブだけを切り取った新しいセッションが作成されます。

#### セッションの削除
次の手順でセッションを削除することができます。
1. セッションマネージャーから**削除したいセッションの名前**をクリックします。
1. セッションの右側にある**「...」**をクリックし、削除を選択します。
1. 確認画面が表示されるので「OK」を選択します。この操作はキャンセルすることができないため、本当に削除してよいセッションなのかよく確認しましょう。

#### 使い方のヒント
セッション機能の使い方は人によって大きく異なることでしょう。**毎日練習を始めるときに新しくセッションを作成してAo100それぞれ測定する人**もいれば、**3x3x3のソルブを全て保存するためのセッションをひとつだけ使っている人**もいるでしょう。セッションの使い方に正解はありません！

- **練習のたびにセッションを作る。** 毎日新しくセッションを作成して練習を始める。時々セッションをまとめてマージして、一週間や一ヶ月単位などのセッションを作って保存しておく。後から見返したときに「その期間はこんなタイムだったのか」とわかりやすい
- **同じスクランブルタイプでは1つのセッションだけを使う。** セッションを作成／マージする手間がない。数万ソルブが溜まっていくことになるので「こんなに練習したぞ！」という達成感を得やすい
- **各ステップを練習するためだけのセッションを作る。** Crossのみ、Cross+F2Lのみ、など。

セッションのインポートとエクスポートについて記載予定
{: .notice--danger}

### ツール {#tools}
{% include gallery id="gallery_tools" caption="ツール" %}

ツールの利用、各ツールの機能と利用方法について記載予定
{: .notice--danger}

### キーボードショートカット {#keyboad-shortcuts}
主要なキーボードショートカットは以下の通りです。
- `Space`: タイマーのスタート、ストップ
- `Ctrl + 1`: 最後のタイムをOKにする
- `Ctrl + 2`: 最後のタイムを+2にする
- `Ctrl + 3`: 最後のタイムをDNFにする
- `Alt + Z`: 最後のタイムを削除する

## オプション {#options}
{% include gallery id="gallery_options" caption="オプション" %}
オプション画面のキャプチャを挿入し、項目ごとに記載予定
{: .notice--danger}

## 高度な機能 {#advanced-features}
- [csTimerを用いた3x3区間タイムの計測とその結果に関する考察 - はたむランド(2014)](http://thereishatamuland.blog34.fc2.com/blog-entry-304.html)
- [スタックタイマーをcsTimerに接続するには - KawamHub(2020)](https://kawam1123.github.io/stacktimer-cstimer-connection/)
- [csTimerのバーチャルキューブ機能 - M'4(2019)](https://kawam1123.hatenablog.com/entry/2019/08/18/082542)

## 外部ツール {#external-tools}
- [kuebiko cubing](http://www.kuebiko-cubing.com/) : csTimerのエクスポートデータを分析するための外部サービス。他のタイマーからのエクスポートデータにも対応しています。

[^1]: csTimerの[多言語翻訳プロジェクト](https://crowdin.com/project/cstimer)にも参加しています。現在の日本語UIのほとんどは私が初稿を書いてます。翻訳に不正確なところや改善点があればご指摘ください。（あるいは翻訳プロジェクトに参加しましょう！）