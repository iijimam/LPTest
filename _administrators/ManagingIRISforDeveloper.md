---
title: 開発者向け InterSystems IRIS の管理概要
date: 2024-12-04
permalink: ManagingIRISforDeveloper.html
layout: post
---
InterSystems IRIS® データプラットフォームとその他のインターシステムズ製品の管理の基本について、ハイレベルな概要を学びます。

このパスは、開発者を対象とした、InterSystems 製品のシステム管理タスク概要を学習できるパスです。

システム管理者向けのより包括的なパスについては、[InterSysetms IRIS 管理の基本](/IRISManagementBasics.html)をご参照ください。

---

[1. <img src="./assets/icons/1.png" width="40%"/>](#1-)

[2. <img src="./assets/icons/d2.png" width="40%"/>](#2-)

[3. <img src="./assets/icons/d3.png" width="40%"/>](#3-)

[4. <img src="./assets/icons/d4.png" width="40%"/>](#4-)

[5. 次は？](#5-次は)

---

## 1. <img src="./assets/icons/1.png" width="70%"/>
InterSystems IRISのアーキテクチャと、システム管理に役立つツールについてご紹介します。


はじめに、InterSystems IRIS概要と、その基盤となる基本アーキテクチャについてご紹介します。

- InterSystems 製品のアーキテクチャ概要 ～ネームスペースとデータベース～

    {% include youtube-list.html id="TNjUnuw8K_Q" list="PLzSN_5VbNaxCWpesN3ulh_EZ9sGkw09q5" %} 

- IRISの開発環境の作成方法、ネームスペース／データベースについて

    IDEからIRISに接続する方法も確認できます。

    ✅ [【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その2：InterSystems IRIS で開発をはじめよう！](https://jp.community.intersystems.com/node/478601)
        
    {% include youtube-list.html id="ID6ImJTgJRk" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %} 


- [ビデオ（英語）：Introduction to the Management Portal](https://learning.intersystems.com/enrol/index.php?id=1322)

- [ビデオ（英語）：Using the InterSystems Terminal](https://learning.intersystems.com/enrol/index.php?id=1433)

    ターミナルで、タイプ：%Status のエラーを受け取った場合の確認方法については、以下[ObjectScriptクックブック](https://github.com/Intersystems-jp/ObjectScriptCookBook)の項目をご参照ください。

    ✅ [%Statusのエラーが戻ってきたら](https://github.com/Intersystems-jp/ObjectScriptCookBook/blob/master/CookBook.md#status%E3%81%AE%E3%82%A8%E3%83%A9%E3%83%BC%E3%81%8C%E6%88%BB%E3%81%A3%E3%81%A6%E3%81%8D%E3%81%9F%E3%82%89)

---

## 2. <img src="./assets/icons/d2.png" width="70%"/>

ユーザーを作成し、対応するロールに接続することで、必要なものにはロールベースでアクセスできるようにし、ロールに関係のないデータやツールへのアクセスを禁止します。次に、データベースを暗号化することで安全なデータを確保する方法をご覧ください。

- [ビデオ（英語）：Users and Roles in InterSystems IRIS](https://learning.intersystems.com/course/view.php?name=Users%20Roles%20IRIS)

    日本語字幕なし（付けてもいいかも）

- [演習環境付き演習（英語）:Configuring Role-Based Access](https://learning.intersystems.com/enrol/index.php?id=2157)

    演習の例では、管理ポータルで使用する 2 種類のマネージャ・ロールの設定方法を示しています。最初のロールは、ユーザ定義やロール定義などのセキュリティ関連項目の変更を許可するページにアクセスできます。2つ目のロールにはそのようなアクセス権はありません。また、これらのロールを持つユーザが管理ポータルとどのようにやり取りするかも説明します。なお、LDAP もサポートされていますが、この演習では取り上げません。

- [ドキュメント：暗号化](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=ROARS_encrypt)

---
## 3. <img src="./assets/icons/d3.png" width="70%"/>
ログを使用してエラーを早期に特定し、問題をトラブルシューティングする方法をご覧ください。

### アプリケーションエラーログ

- [記事：メッセージ・ログ(messages.log)／コンソール・ログ(cconsole.log) に出力される「Purging Application Error Logs」のメッセージとは](https://jp.community.intersystems.com/node/508271)

- [記事：アプリケーションのログを^ERRORSグローバルに入れる方法](https://jp.community.intersystems.com/node/508466)

> **英語ビデオやオンラインコースもあります**
>
>- [ビデオ（英語）:Reviewing the Application Error Log](https://learning.intersystems.com/enrol/index.php?id=1131)
{: .block-tip}

### SYSLOG

- [記事：SYSLOG - その正体と意味するもの](https://jp.community.intersystems.com/node/492146)

> **英語ビデオやオンラインコースもあります**
>
>- [ビデオ（英語）:Reviewing the Console Log and SYSLOG](https://learning.intersystems.com/course/view.php?id=1133)
{: .block-tip}

### トラブル時の情報収集

- [ドキュメント：InterSystems 診断レポートの使用法](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCM_diagnostic)

    概要のみお読みください

✅ [記事＋日本語ビデオ：【IRISベース】トラブル発生時の情報収集方法（IRIS ／ IRIS for Health ／ UCR 編）](https://jp.community.intersystems.com/node/489511)

{% include youtube-list.html id="yFmpQFkErwI" list="PLzSN_5VbNaxCeC_ibw2l-xneMCwCVf-Or" %}  


✅ [記事＋日本語ビデオ:【Caché ベース】トラブル発生時の情報収集方法（Caché ／ Ensemble ／ HealthConnect 編）](https://jp.community.intersystems.com/node/489516)

{% include youtube-list.html id="lW1ghMpURlM" list="PLzSN_5VbNaxCeC_ibw2l-xneMCwCVf-Or" %}  


- [ドキュメント：irisstat ユーティリティを使用した InterSystems IRIS の監視](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCM_irisstat)

- [ドキュメント：緊急アクセス](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=ROARS_gsecuring_secmgmt#ROARS_gsecuring_secmgmt_emerg)

- Webアプリで障害が発生した場合の対応例

    [記事「Webアプリケーションのトラブルシュート方法（ログの取得方法）」](https://jp.community.intersystems.com/node/548871)

**※ 問題が解決しない場合は、システムはそのままで「診断レポート」または「^SystemCheckまたは^Buttons」を実行し、インターシステムズのサポートセンターまでお問い合わせください。**

---

## 4. <img src="./assets/icons/d4.png" width="70%"/>
冗長性と自動監視を組み込むことで、システムを効果的に稼働させ続ける方法を学びましょう。

### バックアップとリストア（シリーズ記事）

- [インターシステムズ製品をバックアップする前に確認したいこと](https://jp.community.intersystems.com/node/566721)

- [外部バックアップの仕組みとバックアップとリストア方法について](https://jp.community.intersystems.com/node/566816)

- [オンラインバックアップの仕組みとバックアップとリストア方法について](https://jp.community.intersystems.com/node/566936)

- [並行外部バックアップの仕組みとバックアップとリストア方法について](https://jp.community.intersystems.com/node/567071)

- [コールドバックアップとリストア方法について](https://jp.community.intersystems.com/node/567076)

> **英語ビデオやオンラインコースもあります**
>
>- [オンラインコース(英語）:Backup and Restore](https://learning.intersystems.com/course/view.php?name=Backup%20and%20Restore)
>
>InterSystems IRIS® データ・プラットフォーム・システムのバックアップとリストアの方法、および効果的なバックアップ戦略の設計について説明します。
>
>   前提学習または経験：管理ポータルおよび InterSystems IRIS の一般的なアーキテクチャについての理解が必要です。
>   
>    学習目標 このコースを修了するまでに、以下のことができるようになります：
>
>    - 外部バックアップ・ソフトウェアまたは仮想マシンのスナップショットを使用して、InterSystems IRIS 内をバックアップする利点と欠点を識別する。
>    - サイトの効果的なバックアップ戦略を設計する
>    - 外部ツールを使用したInterSystems IRISのバックアップとリストア
>
>    >このオンラインコースは実際の演習は含まれていません。
{: .block-tip}

---
## 5. 次は？
学習を継続する場合は以下のリソースが最適です。

- [演習環境（英語ページ）:Performing Common InterSystems IRIS Management Tasks](https://learning.intersystems.com/enrol/index.php?id=1945)

    IRISのインストールをお試しいただけます（Ubuntuを利用）。また、インストール後にデータベースキャッシュサイズとジャーナル設定をいくつか変更します。

- [ラーニングパス：InterSysetms IRIS 管理の基本](/IRISManagementBasics.html)

- [ドキュメント：管理](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=PAGE_administration)
