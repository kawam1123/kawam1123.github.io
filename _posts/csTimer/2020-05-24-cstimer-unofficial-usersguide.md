---
title: csTimer日本語版ユーザーズガイド(非公式)
excerpt: csTimerはスピードキューブ用のオンラインタイマーアプリです。本ドキュメントはcsTimerの日本語版の非公式ユーザーズガイドです。日本語版UIをベースに、主な機能と操作方法について解説します。（スクランブル、統計情報、ソルバー、バックアップなど）
description: csTimerはスピードキューブ用のオンラインタイマーアプリです。本ドキュメントはcsTimerの日本語版の非公式ユーザーズガイドです。日本語版UIをベースに、主な機能と操作方法について解説します。（スクランブル、統計情報、ソルバー、バックアップなど）
date: 2020-05-26 22:00:00 +0900
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
  - url: /assets/img/cstimer/cstimer_statmenu.png
    image_path: /assets/img/cstimer/cstimer_statmenu.png
    alt: "統計情報メニュー"
    title: "統計情報メニュー"
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
  - url: /assets/img/cstimer/cstimer_tool_draw.png
    image_path: /assets/img/cstimer/cstimer_tool_draw.png
    alt: "スクランブルの描画"
    title: "スクランブルの描画"
  - url: /assets/img/cstimer/cstimer_tool_crosssession.png
    image_path: /assets/img/cstimer/cstimer_tool_crosssession.png
    alt: "クロスセッションの統計情報"
    title: "クロスセッションの統計情報"
  - url: /assets/img/cstimer/cstimer_tool_solver.png
    image_path: /assets/img/cstimer/cstimer_tool_solver.png
    alt: "ソルバー"
    title: "ソルバー"
  - url: /assets/img/cstimer/cstimer_tool_dailystat.png
    image_path: /assets/img/cstimer/cstimer_tool_dailystat.png
    alt: "Daily Statistics"
    title: "Daily Statistics"

gallery_quickstart:
  - image_path: /assets/img/cstimer/cstimer_quickstart1.png
  - image_path: /assets/img/cstimer/cstimer_quickstart2.png
  - image_path: /assets/img/cstimer/cstimer_quickstart3.png
  - image_path: /assets/img/cstimer/cstimer_quickstart4.png

---
本記事は書きはじめたばかりです！とりあえず雛形だけ作った状態なので、まだ内容はあまりありません(2020/05/24)
{: .notice--info}

## 本ユーザーズガイドについて {#about}
![](/assets/img/cstimer/cstimer_screenshot.png){:width="600px" height="auto" class="img-responsive align-center"}

本ユーザーズガイドは、**スピードキューブ用オンラインタイマーアプリケーション「csTimer」日本語版の機能をまとめて解説するためのものです。** 開発者に許諾を得たものではなく、日本語版UIに準拠して独自に紹介をするものです。ここに記載されている情報は正確でない場合があります。

csTimerは中国のスピードキューバー[Shuang Chen (cs0x7f)](https://www.speedsolving.com/wiki/index.php/Shuang_Chen)によって2012年にリリースされたスピードキューブ用のオンラインタイマーアプリケーションです。2020年05月現在もアクティブに機能追加や修正が進められており、スピードキューブの計測用のタイマーとして必要な基本的機能が揃っているだけでなく、他のタイマーアプリにないような機能も豊富にあります。それぞれの機能の概要や使い方についてまとめたものがなかったため、非公式にユーザーズガイドを執筆することにしました。本ドキュメントがcsTimerユーザーの助けになれば幸いです。[^1]

## クイックスタート {#quickstart}
まずは、まったくcsTimerを使ったことがない人向けとして、計測を始めるまでの流れを簡単にお教えしましょう。（csTimerを使ったことのあるユーザーは読み飛ばしてください！）

**csTimerはスピードキューブの練習用に作られたタイマーアプリケーションです。**主にルービックキューブ(3x3x3キューブ)を速く解くための練習に使われますが、他にもいろいろな競技に対応しています。Webブラウザ上で動作するので、プラットフォームを選ばず利用することができます。PC/Mac/Linux/iOS/Androidのどの環境でも同じように動作します。さあ、次の手順に従って使ってみましょう！

1. **[https://cstimer.net](https://cstimer.net)にアクセスします。**モダンなブラウザ(Chrome、Firefox、Edgeなど)であれば問題なく動作するでしょう。 次のような初期画面が表示されれば成功です。 
![](/assets/img/cstimer/cstimer_quickstart1.png){:width="600px" height="auto" class="img-responsive align-center"}  
![](/assets/img/cstimer/cstimer_quickstart_mobile.png){:width="300px" height="auto" class="img-responsive align-center"}
2. **画面上部にルービックキューブ(3x3x3キューブ)のスクランブルが表示されています。**まずはスクランブルに従ってキューブを崩してみましょう。スクランブルが読めない？回転記号がわからない？そんなあなたはまず[ここ](https://cubevoyage.net/how-to-solve/intermediate/notation/)や[ここ](https://tribox.com/3x3x3/solution/notation/)を読みましょう。
3. キューブを無事にスクランブルできたら、**キーボードのスペースキーを長押しします。スマートフォンやタブレットを使っている場合は、画面の真ん中あたりを長くタップしましょう。** このとき、次のような画面に変わるはずです。  
![](/assets/img/cstimer/cstimer_quickstart3.png){:width="600px" height="auto" class="img-responsive align-center"}
4. **スペースキーを離すと計測が開始します。**スマートフォンやタブレットではタップした指を離すだけです。さあ急いでキューブを解き始めましょう！できる限り速く！
![](/assets/img/cstimer/cstimer_quickstart4.png){:width="600px" height="auto" class="img-responsive align-center"}
5.無事にキューブを揃えられましたか？では、**スペースキーをもう一度軽く押してタイマーを止めましょう。** スマートフォンやタブレットではタップします。画面右側のタイム一覧にあなたのタイムが新しく追加されているのがわかるでしょうか？ **これでcsTimerでの初計測は無事終了しました！おめでとうございます！**  
![](/assets/img/cstimer/cstimer_quickstart5.png){:width="600px" height="auto" class="img-responsive align-center"}
6. 何度か計測をしていくと、左側の統計パネルに**Ao5やAo12などの統計情報が自動的に表示されていくのがわかるでしょう。** タイムの分布やヒストグラムを表示するツールと使って、あなたのタイムを可視化することもできます。**画面左上にあるメニューから「ツール」ボタンを選択して、「タイムの分布」や「タイムトレンド」などのツールを使ってみましょう。**  
![](/assets/img/cstimer/cstimer_menu.png){:width="600px" height="auto" class="img-responsive align-center"}  
![](/assets/img/cstimer/cstimer_quickstart6.png){:width="600px" height="auto" class="img-responsive align-center"}
7. **計測されたタイムのデータは自動的にブラウザ内に保存されます。**ブラウザのキャッシュを削除しない限りデータは消えませんが、データが消えないようにしておきたいなら、定期的にバックアップすることをお勧めします。**メニューから「エクスポート」ボタンを選択して、データの保存先を選択しましょう**（自動的にエクスポートするオプションもあります）。
![](/assets/img/cstimer/cstimer_quickstart7.png){:width="600px" height="auto" class="img-responsive align-center"}  
8. さあ、次は何をしましょう。4x4x4の練習をしてWRを取りたい？スクエア-1の成形(CSP)だけを練習してsub-10したい？3x3x3複数目隠しで1時間を無駄にしたい？ 次に何をするかはあなた次第です。  
**csTimerをお楽しみください！**

## 主要機能は？ {#features}
csTimerの主要機能および操作方法を説明します。

### スクランブル {#scramble}
csTimerは、**全てのWCA公式種目のスクランブルに対応(WCA準拠）**しており、スピードキューブ練習のためのスクランブル、計測、記録、統計表示の機能がひとつにまとまっています。また、特定のサブステップを練習するためのスクランブルや、リレー競技(234リレーなど)、エッジのみ、コーナーのみ、簡単なクロス、など、非常に多くのスクランブルタイプを選択することができます。

また、「3x3x3」と「3x3x3片手」など、まったく同じアルゴリズムでスクランブルを生成するものもあります。実施する競技に応じてスクランブルタイプを設定することで、同じ種類のスクランブルをまとめて統計情報を表示することができます。（例・複数のセッションから3x3x3片手の記録だけ抜き出して統計を表示したい）

対応しているスクランブルタイプの例を以下に挙げます。
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
- 3x3x3複数目隠し（キューブの個数を指定可能）

#### 特定のサブステップを練習するためのスクランブル
- F2L
- OLL
- PLL
- ZBLL (ZB)
- ZBLS (ZB)
- ZZLL (ZZ)
- EOLine (ZZ)
- L2E (Roux)
- L2E <M,U> 2gen (Roux)
- L10P (Roux)
- ラストレイヤーのエッジのみ
- ラストレイヤーのコーナーのみ
- エッジのみ
- コーナーのみ
- イージークロス（指定した手数で揃えられるクロス）
その他多数

#### スクランブルタイプの変更
**スクランブルのタイプを変更するには、画面上部のスクランブルパネルからカテゴリー／サブカテゴリーのドロップダウンメニューを選択します。**スクランブルのカテゴリーを切り替えると、自動的にサブカテゴリーの内容が変更されます。スクランブルによっては、オプションを指定することができます。（例・イージークロスの手数、3x3x3複数目隠しの挑戦個数、スクエア1の成形パタンなど）

![](/assets/img/cstimer/cstimer_scramble_panel.png){:width="800px" height="auto" class="img-responsive align-center img-thumbnail"}

- カテゴリーとして`WCA`を選択すると、サブカテゴリーにはWCA公式種目の名称が表示されます。
- カテゴリーとして`3x3x3`を選択すると、サブカテゴリーには3x3x3のサブステップを生成するためのスクランブルが表示されます。たとえば、ここで`OLL`や`PLL`を選択すると、ランダムなOLL/PLLを練習するためのスクランブルになります。  
![](/assets/img/cstimer/cstimer_3x3x3_sub.png){:width="200px" height="auto" class="img-responsive align-center img-thumbnail"}
- このとき、**「スクランブルのオプションを指定」**ボタンを押せるようになっていれば、追加のオプションを指定することができます。たとえば、OLLを選択した場合、**特定のOLLケースのみがランダムに出現するスクランブル**を出力することができます。  
![](/assets/img/cstimer/cstimer_oll.png){:width="800px" height="auto" class="img-responsive align-center img-thumbnail"}

### 統計機能 {#stat}
Ao5やAo12などの基本的な統計機能のほか、セッション単位でのソルブ管理、区間タイムの計測機能（マルチフェイズ機能）などが含まれます。

#### 現在のラウンドの統計情報
![](/assets/img/cstimer/cstimer_statmenu.png){:width="600px" height="auto" class="img-responsive align-center img-thumbnail"}

基本的な統計情報は画面左側の**「現在のラウンドの統計情報」**に表示されます。  
デフォルトの統計指標は`Mo3 Ao5 Ao12 Ao25 Ao50 Ao100`です。下記のオプションから、自分の表示したい指標を選択することができます。プルダウンメニューに表示されていない指標もカスタムで入力することができます。Ao1000やAo10000を表示させたいときにはこのオプションを変更しましょう。

- `[オプション]>[統計情報]>[カスタム統計指標]`

また、画面左下のタイム一覧では、個別のタイムと合わせて指定した2つの指標を確認することができます。デフォルトでは**個別タイム、Ao5、Ao12**が表示されます。ここに表示される統計情報は下記のオプションから変更することができます。特定のセッションでのみ、Ao5とAo100を表示しておくという使い方もできるでしょう。

- `[オプション]>[統計情報]>[リスト1の種類](average|mean)`
- `[オプション]>[統計情報]>[リスト1の長さ](3-1000)`
- `[オプション]>[統計情報]>[リスト2の種類](average|mean)`
- `[オプション]>[統計情報]>[リスト2の長さ](3-1000)`

#### クロスセッションの統計情報
**セッションが複数に分かれるとき、同じスクランブルタイプに絞って統計情報を表示することができます。** メニューから「ツール」を選択し、「クロスセッションの統計情報」を選択しましょう。
![](/assets/img/cstimer/cstimer_tool_crosssession_menu.png){:width="400px" height="auto" class="img-responsive align-center img-thumbnail"}
ここでは次の３つのドロップダウンメニューを使って、表示するソルブの範囲を絞ることができます。

- **セッション**：対象セッションを選択する。セッションの一覧から選択するか、全セッションを選択する。
- **期間**：対象期間を選択する。指定の期間（24時間、7日、30日、356日）から選択するか、全期間を選択する。
- **スクランブル**：これまでにソルブしたスクランブルタイプから選択するか、全スクランブルから選択する。

すると、指定した条件に応じて、複数のセッションにまたがって統計情報が計算され、次のように表示されます。

![](/assets/img/cstimer/cstimer_tool_crosssession.png){:width="600px" height="auto" class="img-responsive align-center img-thumbnail"}

#### 区間タイムの計測（マルチフェイズ）
**マルチフェイズ機能は、ひとつのソルブのタイムを分割して計測することができる機能です。** これは下記のメニューからセッションごとに設定します。分割したいフェイズの数を入力しましょう。たとえば、CFOPの各手順についてそれぞれ計測したいのなら、4 (Cross、F2L、OLL、PLL)を入力しましょう。フェイズを分割せずに計測する場合は1を入力してください。

`[オプション]>[タイマー]>[マルチフェイズ(1~10)]`

この設定が有効になった状態で計測を開始するときは、いつものように計測を開始して、次のフェイズに入った段階でスペースキーを軽く叩きましょう。すると、**それぞれのフェイズごとのタイムが自動的に計測され、画面の左側に表示されます。これをフェイズの数だけ繰り替えすと、タイマーが停止し、タイムが保存されます。**
![](/assets/img/cstimer/cstimer_multiphase_input.png){:width="400px" height="auto" class="img-responsive align-center img-thumbnail"}

ここで計測したフェイズごとのタイムはタイム一覧にも表示されます。P.1から順にフェイズの数だけ列が追加、フェイズごとのMeanが表示されます。現在のラウンドの統計情報の「time」をクリックすると、フェイズごとのAo5やAo12を確認することもできます。

![](/assets/img/cstimer/cstimer_multiphase_stat.png){:width="400px" height="auto" class="img-responsive align-center img-thumbnail"}

この機能は様々な用途に使えますが、次のような場合に使うと便利でしょう。

- **CFOPのステップ(Cross、F2L、OLL、PLL)ごと**のタイムを計測し、自分の苦手なステップを特定する。また、集中的に練習する。CFOPに限らず、RouxでもYauでもReductionでも、自分が使っているメソッドをステップごとに分けて練習するのに使えるでしょう。[^CFOP-split]
- **3x3x3目隠し競技などで、分析・記憶のフェイズと実行のフェイズをそれぞれ分けて計測する。** 分析が速かったけれど実行がダメだった、分析をあと10秒短くしたい、などの目標を明確にするのに役立ちます。
- **2-7リレー**などでそれぞれのパズルごとのタイムを計測する。リレー競技をやりたいときのためのスクランブルも生成できますので、リレー競技者にはたまらないでしょう。
- **複数人でリレー競技をやるときに、人数分のフェイズに分割しておき、それぞれの参加者のタイムを計測する。**3x3x3目隠しリレー(BLDリレー)などで便利に使うことができます。何十回もBLDリレーに取り組むときにはこれが心の支えになるかもしれません。

### セッション管理 {#session-management}
**計測したデータは「セッション」という単位で保存することができます。**タイム一覧を表示しているエリアからセッションマネージャーを使うことができます。セッションごとに名前をつけて、スクランブルタイプ(3x3x3、4x4x4など)、統計情報(Ao5/Ao12/Ao100など)、フェイズ数(分割数)が管理できます。
{% include gallery id="gallery_sessions" caption="セッションマネージャー" %}

各セッションのタイム一覧に表示された個別のタイムをクリックすることで、そのソルブの詳細を表示することができます。ソルブの詳細には次の内容が含まれています。

![](/assets/img/cstimer/cstimer_solvedetail.png){:width="800px" height="auto" class="img-responsive align-center img-thumbnail"}

- そのセッションの中でのソルブの番号
- タイム (マルチフェイズが有効になっている場合は、分割して表示される)
- ソルブのコピー
- ペナルティの有無 (OK、+2、DNF)
- コメント
- スクランブル
- 日時
- 実際のムーブ (alg.cubing.netへのリンク。バーチャルキューブなどを利用した場合のみ表示)

**タイマーを止めたときにソルブが完成状態ではないときは、ペナルティ(+2あるいはDNF)を入力しましょう。**各WCA公式パズルの完成状態については、[こちらのWCA規則](https://www.worldcubeassociation.org/regulations/translations/japanese/#article-10-solved-state)を参照してください。[キーボードショートカット](#keyboad-shortcuts)を使って入力するのが便利です。

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

### ソルバー {#solver}
クロス、X-Cross、2x2x2の一面、スキューブの一面、スクエア1の整形などのソルバー機能があります。クロスなど特定のステップの学習や練習に利用できます。
### バックアップ {#backup}
計測したデータは自動的にブラウザ内のデータベースに保存されますので、データを手動で保存する必要はありません。このデータはエクスポート／インポートすることができます。これはcsTimerの非常に便利な機能のひとつで、**複数の端末を使い分けて計測する場合でも、すぐに最新のソルブデータや設定情報を読み込んで練習を始めることができます！**

特に、クラウドストレージにエクスポート／インポートすることができるため、使っているマシンが壊れたとしてもデータを全て失うことはありません。また、ソルブデータやアプリケーション実体は、キャッシュ上に展開されるため、インターネット接続がなくても計測をすることができます。

![](/assets/img/cstimer/cstimer_export_initial.png){:width="auto" height="auto" class="img-responsive align-center img-thumbnail"}

**[データのインポート／エクスポート]**のメニューから、4種類のバックアップ先を選択することができます。このときエクスポート／インポートされるデータは、全セッションの全ソルブデータになりますので、注意してください。特定のセッションのデータのみインポート／エクスポートしたい場合は、セッションマネージャーの画面から実施しましょう。

- サーバー (WCAID連携)
- サーバー (Google Drive)
- サーバー (csTimerサーバー)
- ローカルファイル (txt形式)

#### サーバー(WCAID連携)
**WCAアカウントと連携して、csTimerサーバー上にデータを保存することができます。** WCAアカウントとは、WCA公式大会に参加する際に必要になる `www.worldcubeassociation.org` のログインアカウントのことです。ただし、このアカウントは公式大会に参加した経験がなくても無料で取得することができます。csTimerに限らず、スピードキューブ関連のWebツールの中にはWCAアカウントでログインすると自動的に連携できるものがあるので、取得しておいて損はないでしょう。

`[データのインポート／エクスポート]`>`[WCAアカウントでログイン]` をクリックすると、`https://www.worldcubeassociation.org/users/sign_in` のページにリダイレクトします。この画面でWCAアカウントでログインしましょう。持っていない人は画面下部の「アカウント登録」から新規作成できます。

![](/assets/img/cstimer/cstimer_wca_login.png){:width="auto" height="auto" class="img-responsive align-center img-thumbnail"}

ログインが成功するとcsTimerの画面に戻り、自分のWCAIDと名前が表示されるようになります。「サーバーからインポート」と「サーバーにエクスポート」のボタンが表示されるようになれば、連携は完了です。**「サーバーにエクスポート」をクリックして、ソルブのデータと設定内容をエクスポートすることができます。**

![](/assets/img/cstimer/cstimer_wca_login_success.png){:width="auto" height="auto" class="img-responsive align-center img-thumbnail"}

#### サーバー (Googleアカウント連携)
上記のWCAID連携と同じように、**Googleアカウントと連携してGoogle Drive上にデータを保存することができます。** 保存されたデータはGoogle Drive上のappDataFolderという領域に保存され、csTimerアプリケーションからしかアクセスできないようになります。自分自身でGoogle Driveの画面から確認することはできません(APIを利用すればもちろんできます)。

`[データのインポート／エクスポート]`>`[Googleアカウントでログイン]` を選択して、自分のGoogleアカウントでログインしましょう。必要なリソースにアクセスするための許可をすれば連携は完了です。WCAID連携と同じように、「サーバーにエクスポート」をクリックして、ソルブのデータと設定内容をエクスポートすることができます。

また、ローカルのエクスポート／インポート機能があり、kuekibo-cubingのような外部ツールと連携して自分のソルブを分析することができるでしょう。

#### サーバー (csTimer)
これは上記2つのエクスポート機能と比べると少し簡易的な機能です。**あなたのアカウント名を指定して、csTimerサーバー上にソルブのデータを保存しておくことができます。** 利用できる文字は英数字のみです。ここで入力したアカウント名をキーとしてデータを保存してくれていると考えるといいでしょう。

![](/assets/img/cstimer/cstimer_export_cstimer.png){:width="auto" height="auto" class="img-responsive align-center img-thumbnail"}

データをインポートするときには、入力したアカウント名と同じものを入力する必要があります。このとき、**特にセッションの判定などはされませんので、他のユーザーであっても同じ文字列を入力すればあなたのソルブのデータを取得することができます。** あまりないとはおもいますが、ソルブごとのコメント欄などに機微な情報を書いている場合は、WCAアカウントやGoogleアカウントと連携したエクスポート／インポート機能を使うとよいでしょう。

#### ローカル
**ローカルのストレージにデータをダウンロードすることができます。**ファイル形式はなぜかtxt形式(UTF-8N)であり、データの形式はjsonフォーマットに従っています。このデータを自分自身でパースして統計データを作ってもよいでしょうし、別のタイマーにデータをインポートできる形に成形してもよいでしょう。また、[kuebiko cubing](http://www.kuebiko-cubing.com/)のような外部ツールを使って、自分自身のソルブを解析してみるのも楽しいでしょう。

ソルブの数が非常に多いとファイルを開くだけでも時間がかかるかもしれません。jsonをフォーマットして読み取れるエディタで開くことを推奨します。

それぞれのセッションごとのデータをエクスポートするときは、csv形式でダウンロードされます。

#### 他のタイマーからセッションをインポート
これはインポート専用の機能です。csTimerからのエクスポートデータをインポートできるのは当然ですが、サポートされている他のタイマーからのセッションデータをインポートすることができます。2020年6月時点で対応しているタイマーは下記の通りです。これらのタイマーにはセッションのエクスポート機能があります。（タイマーによっては予告なくエクスポート機能が削除される場合があります）

- ZYXTimer (iOS/Android)
- TwistyTimer (Android)
- BlockKeeper (Win/Mac/Linux)
- PrismaTimer (Win/Mac)
- DCTimer (raw/sqlite) (iOS)
- Cube Timer (mateus.cubetimer) (Android)

ここには記載はありませんが、対応していないタイマーデータをcsTimerのデータと同じ形式に成形してインポートすることも可能です。csTimerのデータ形式をよく観察して、色々なタイマーのデータをインポートしてみるとよいでしょう！
{: .notice--info}

#### 設定内容のエクスポート／インポート
設定内容のみエクスポート／インポートすることもできます。下記のどちらかのメニューを選択することで、現在設定されているオプションの内容をエクスポートすることができます。

- `[データのインポート／エクスポート]`>`[オプションのみエクスポート／インポート]`
- `[オプション]`>`[エクスポート]`

ここで表示されたテキストボックスに、過去にエクスポートしたテキストを張り付けることで、設定されているオプションを復元することができます。

![](/assets/img/cstimer/cstimer_export_options.png){:width="auto" height="auto" class="img-responsive align-center img-thumbnail"}

#### エクスポート／インポート時の注意事項
繰り返しになりますが、この機能でエクスポート／インポートされるデータは、**全セッションの全ソルブデータが対象となります。** エクスポート先が同じ場合、データが上書きされる場合がありますので、現在のデータを本当に保存していいのか、確認してから実行しましょう。

**特に、データをインポートするときには最大限の注意をはらうといいでしょう。** 最新のデータだろう！と思ってインポートしたデータが最新ではなかった、ということが非常に起こりやすいです。大切なソルブのデータを失わないためにも定期的なデータのバックアップを取ることをお勧めします。また、誤ってデータを上書きしてしまったときのために、ローカルにもデータをエクスポートしておくといいでしょう。

一定のソルブごとにデータを自動的にエクスポートする機能もあります。`[グローバル]>[オートエクスポート]>[WCAアカウントに保存]`を有効にしておくと、データ喪失の危険性がだいぶ減るでしょう。

## 基本操作 {#basic-usage}
### UI {#user-interface}
{% include gallery id="gallery_ui" caption="ユーザーインターフェイス" %}

ユーザーインターフェイスの詳細について記載予定
{: .notice--danger}

### タイマー {#timing}
スペース、インスペクションあり、タイピング、スタックタイマー連携



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
- `Alt + I`: スクランブルタイプを「入力」に変更する

## オプション {#options}
{% include gallery id="gallery_options" caption="オプション" %}
オプション画面のキャプチャを挿入し、項目ごとに記載予定
{: .notice--danger}

### よくある質問 {#faq}
#### Q.ブラウザのキャッシュを消したらタイムが全部消えちゃった！どうしよう？
A. **csTimerの記録はブラウザ内のデータベースに格納されていますので、キャッシュを消してしまうとデータがなくなってしまいます！**記録を失いたくなければ、定期的にデータのバックアップをしましょう。また、100ソルブごとに自動的にクラウドストレージにデータをバックアップする機能[^auto-export]もありますので、是非お使いください。

また、あなたがアクセスしているのは本当にいつも使っているcsTimerのアドレス (`https://cstimer.net`) ですか？csTimerはオープンソースソフトウェアなので、いくつかのクローン（コピー）が存在します。正しいサイトにいることを確認しましょう。もしかするとhttp/httpsの入力を間違っているだけかもしれません。

#### Q.セッションやスクランブル、ツールのドロップダウンメニューが消えちゃった！どうしよう？
A. タイム一覧、スクランブル、ツールの**左上のコーナーには小さなボタンがあります。**このボタンを押すとそれぞれの要素のメニューの表示／非表示を切り替えることができます。間違って消してしまってもびっくりしないように！画面上に表示されるものを少なくしたいときには非表示にしておいてもいいでしょう。

#### Q.セッションごとに設定を変えたいんだけど？
A. **「オプション」を開いて右端にある「セッションごと」の列のチェックボックスをつけましょう。**チェックボックスがONになっている設定項目はセッションごとに独立して管理されます。全体で管理される設定項目にはチェックボックスが表示されません。

#### Q.バーチャルキューブ機能を使うには？
A.下記のメニューから設定できます。

- (日本語) **[オプション]>[タイマー]>[タイム入力方式]>[バーチャルキューブ]を選択する**  
- (英語) **[Option]>[timer]>[entering in times with]>[virtual]を選択する**

バーチャルキューブ機能の詳細は[こちら](https://kawam1123.hatenablog.com/entry/2019/08/18/082542)を参照してください。

#### Q. 別のタイマーで生成したスクランブルでソルバーを使いたい
A. ソルバーで「クロス」を選択し、スクランブルのタイプを「入力」に変更して、そこにスクランブルをペーストしましょう。キーボードショートカットAlt+Iでも変更できます。他のソルバーも使えますので、オンライン大会のスクランブルでDRを探すのに使ったりもしましょう。

#### Q. csTimerの配色やデザインを変更したい
A. UIのデザインは `[オプション]>[表示]`の下記項目から変更できます。

- `[タイマーフォントの選択]`: タイマーのフォントを変更できます
- `[UIデザイン]`: マテリアルデザインや影なしデザインに変更できます
- `[UIスタイル]`: デスクトップ表示とモバイル表示を切り替えます。通常は「自動」を選択しておけばいいでしょう
- スクランブルパネル、統計パネル、ツールパネルの表示スタイルもそれぞれフラットデザインを指定することができます。

配色については、`[オプション]>[色]`からそれぞれの要素の色、キューブの配色を変更できます。  
デフォルトの配色に戻したい場合は、`[カラーテーマの選択]`から「スタイル１」を選択しましょう。  
また、`[概要]>[配色]`からあらかじめ用意された配色を利用することができます。下記のようなリンクを生成して、自分の配色を共有することもできます。(https://cstimer.net/#fff#023#034#b80#28d#678#034)

また、`[オプション]>[表示]>[背景画像]`(デフォルト:なし)から背景画像を指定することができます。csTimerにあらかじめ登録された画像のほか、外部の画像URLを指定して背景画像として利用することもできます。  
`[背景画像の透過度(0~100)]`(デフォルト:25)で透過度を指定できます。

## 高度な機能 {#advanced-features}
- [csTimerを用いた3x3区間タイムの計測とその結果に関する考察 - はたむランド(2014)](http://thereishatamuland.blog34.fc2.com/blog-entry-304.html)
- [スタックタイマーをcsTimerに接続するには - KawamHub(2020)](https://kawam1123.github.io/stacktimer-cstimer-connection/)
- [csTimerのバーチャルキューブ機能 - M'4(2019)](https://kawam1123.hatenablog.com/entry/2019/08/18/082542)

## 外部ツール {#external-tools}
- [kuebiko cubing](http://www.kuebiko-cubing.com/) : csTimerのエクスポートデータを分析するための外部サービス。他のタイマーからのエクスポートデータにも対応しています。

[^1]: csTimerの[多言語翻訳プロジェクト](https://crowdin.com/project/cstimer)にも参加しています。現在の日本語UIのほとんどは私が初稿を書いてます。翻訳に不正確なところや改善点があればご指摘ください。（あるいは翻訳プロジェクトに参加しましょう！）
[^auto-export]: `[グローバル]>[オートエクスポート]>[WCAアカウントに保存]`がオススメです。
[^CFOP-split]: 自分のCFOPのタイムをステップごとに分割したときに、どのステップに課題があるのかを知ることができるでしょう。この用途に限っていえば、**CubeSkillsで[CFOP Solve Splits Tool](https://www.cubeskills.com/blog/cfop-solve-splits-tool)という素晴らしいツールが公開されています。**これは自分のCross-F2L-OLL-PLLそれぞれのタイムを入力すると、平均的なソルブと比較してどこに課題があるかを可視化してくれるツールです。ぜひ使ってみましょう！　ちなみに、私は「クロスに時間がかかりすぎ！」だそうです。