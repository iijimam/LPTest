---
title: InterSysetms IRIS 管理の基本
date: 2024-12-03
permalink: IRISManagementBasics.html
---
> オリジナル:[InterSystems IRIS Management Basics](https://learning.intersystems.com/course/view.php?id=1825)

InterSystems IRIS® データプラットフォームの基礎と、システム管理者が製品のライフサイクルを通じて一般的なタスクを実行するのに役立つツールをご紹介します。

このコースを修了すると、通常の操作やトラブルシューティングにインターシステムズのドキュメントを読めばわかる程度の知識が身に付きます。

[1. <img src="./assets/icons/1.png" width="40%"/> ](#1-)

[2. <img src="./assets/icons/2.png" width="40%"/> ](#2-)

[3. <img src="./assets/icons/3.png" width="40%"/> ](#3-)

[4. <img src="./assets/icons/4.png" width="40%"/> ](#4-)

[5. <img src="./assets/icons/5.png" width="40%"/> ](#5-)

[6. <img src="./assets/icons/6.png" width="40%"/> ](#6-)

[7. <img src="./assets/icons/7.png" width="40%"/> ](#7-)

[8. <img src="./assets/icons/8.png" width="40%"/> ](#8-)

[9. <img src="./assets/icons/9.png" width="40%"/> ](#9-)

[10. <img src="./assets/icons/10.png" width="40%"/> ](#10-)

[11. <img src="./assets/icons/11.png" width="40%"/> ](#11-)

[12. 次は？](#12-次は)

---
## 1. <img src="./assets/icons/1.png" width="70%"/>

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

- Interoperability 概要
    - シリーズ記事
    
        - [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：動作の仕組みを知ろう](https://jp.community.intersystems.com/node/487036)

        - [【はじめてのInterSystems IRIS】Interoperability（相互運用性）：プロダクションとは](https://jp.community.intersystems.com/node/487041)


    - ビデオ（20分ごろからご覧ください）

        {% include youtube-list.html id="vo12UnH-c-s" list="PLzSN_5VbNaxD-r8wU4LHwLwGSzUjrffEX&index=1&t=1203s" %}

> **日本語字幕ありの英語ビデオもあります**
>
>✅[ビデオ（英語）:Integration overview:Receiving and Routing Data in a Production](https://learning.intersystems.com/course/view.php?name=Interop%20QS)
{: .block-tip}


- グローバル変数について

    [ガイド：多次元データエンジンの概念およびアーキテクチャ](https://github.com/Intersystems-jp/IRISBasicTechnologyGuide/blob/main/%E5%A4%9A%E6%AC%A1%E5%85%83%E3%83%86%E3%82%99%E3%83%BC%E3%82%BF%E3%82%A8%E3%83%B3%E3%82%B7%E3%82%99%E3%83%B3%E3%81%AE%E6%A6%82%E5%BF%B5%E3%81%8A%E3%82%88%E3%81%B2%E3%82%99%E3%82%A2%E3%83%BC%E3%82%AD%E3%83%86%E3%82%AF%E3%83%81%E3%83%A3.pdf)


> **日本語字幕ありの英語ビデオもあります**
>
>✅[ビデオ（英語）:Exploring Multiple Data Models with Globals](https://learning.intersystems.com/enrol/index.php?id=2189)
{: .block-tip}

---
## 2. <img src="./assets/icons/2.png" width="70%"/>

InterSystems IRIS では、製品をインストールする場所を選択できます。InterSystems IRIS のインストール、インスタンスの起動と停止、基本設定、およびアプリケーションに必要な場合は Web サーバのインストール方法について説明します。

- [ドキュメント：導入](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=PAGE_deployment)

- インストールについて

    ※製品版もコミュニティエディションもインストール方法は同様です。

    ✅ 記事：[【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その１：InterSystems IRIS Community Edition をインストールしてみよう！](【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その１：InterSystems IRIS Community Edition をインストールしてみよう！)

    {% include youtube-list.html id="nKDvM68Gs04" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %}

### コンテナ
InterSystems IRIS コンテナ・イメージからコンテナを開始する方について説明します。

✅ Docker コンテナ版 InterSystems IRIS data platformの勧め

{% include youtube-list.html id="yY8BLUYp5IA" list="PLzSN_5VbNaxAUiQkx5d22TX0zjx4Mmqhb" %}

✅ InterSystems コンテナレジストリの使い方とコンテナ開始までの流れについて

{% include youtube-list.html id="HEGWVP0PIfI" list="PLzSN_5VbNaxAUiQkx5d22TX0zjx4Mmqhb" %}  

✅ まずはコンテナを動かしてみよう！～コンテナ版IRISで新機能を試す方法のご紹介～

{% include youtube-list.html id="JaV3VKWpffs" list="PLzSN_5VbNaxAUiQkx5d22TX0zjx4Mmqhb" %}  

ご参考：[コンテナとIRISについてのYouTubeプレイリスト（日本語）](https://www.youtube.com/watch?v=yY8BLUYp5IA&list=PLzSN_5VbNaxAUiQkx5d22TX0zjx4Mmqhb)

> **英語ビデオもあります**
>
>- ✅[ビデオ（英語）:Docker Containers and InterSystems IRIS](https://learning.intersystems.com/enrol/index.php?id=888)
>   このビデオシリーズでは、Dockerコンテナとその用途を紹介し、InterSystems IRIS®データプラットフォームと組み合わせた場合に、いかに効果的であるかを紹介します。また、コンテナが継続的インテグレーション、継続的デプロイメント（CICD）アプローチにどのように適合するかもご覧いただけます。
>
>- ✅[ビデオ（英語）:Run InterSystems IRIS Community Edition Using Docker](https://learning.intersystems.com/enrol/index.php?id=1762)
>
>- ✅[ビデオ（英語）：Kubernetes Overview](https://learning.intersystems.com/enrol/index.php?id=1753)
>
>     複数のホストにまたがるコンテナのデプロイをオーケストレーションするためのオープンソースプラットフォームであるKubernetesについてご紹介します。InterSystems Kubernetes Operatorにより、InterSystems IRIS®データプラットフォームのユーザは、InterSystems IRISアプリケーションのデプロイメントにおいてKubernetesのメリットを享受することができます。
{: .block-tip}


### ライセンス

- [ドキュメント：InterSystems IRIS ライセンスの構成](https://docs.intersystems.com/irislatestj/csp/docbookj/DocBook.UI.Page.cls?KEY=GSA_license_config)

- [ドキュメント：ライセンス・キーの有効化](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_license_update_key)

---
## 3. <img src="./assets/icons/3.png" width="70%"/>
最初に、ネームスペースとデータベースを作成し、基礎となるデータ構造とどのような関係があるかを学習します。次に、構成パラメータ・ファイル（CPF）、メモリ、およびアラートの構成を学習します。

### システム

- [ドキュメント：InterSystems IRIS インスタンスの制御](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_using_instance_control)

- [ドキュメント：システム情報の構成](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_config_system)

- [ドキュメント：構成パラメータ・ファイルの概要](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=RACS_cpf)

- [コミュニティ：InterSystemsデータプラットフォームとパフォーマンス-パート4: メモリの確認 ](https://jp.community.intersystems.com/node/477746)

- [ドキュメント：Webゲートウェイ概要](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCGI_intro)

> **英語ビデオもあります**
>
>✅[ビデオ（英語）：Configuring the InterSystems Web Gateway](https://learning.intersystems.com/course/view.php?name=ConfigWebGateway)
{: .block-tip}

### ネームスペース

- ドキュメント
    - [ドキュメント：ネームスペースとデータベース](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GORIENT_enviro)

    - [ドキュメント：ネームペースの構成](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_config_namespace)

- ビデオ：ネームスペースとデータベースの作成
    
    ✅[記事：【はじめての InterSystems IRIS】セルフラーニングビデオ：基本その2：InterSystems IRIS で開発をはじめよう！](https://jp.community.intersystems.com/node/478601)

{% include youtube-list.html id="ID6ImJTgJRk" list="PLzSN_5VbNaxBPaSSINLzv-CkDJy00bOSQ" %}  


> **英語ビデオもあります**
>
>✅[ビデオ（英語）：Creating Namespaces and Databases](https://learning.intersystems.com/enrol/index.php?id=2124)
{: .block-tip}


### データベース

- [ドキュメント：ローカル・データベースの作成](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_config_database_create)

- [ドキュメント：データベースの構成](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_config_databases)

- [ドキュメント：ローカルデータベースの管理](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_manage_databases)

---
## 4. <img src="./assets/icons/4.png" width="70%"/>
セキュリティの構成と管理に役立つ製品内のツールと認証オプションを使用して、ユーザーとロールを設定します。

### 概要

- [ドキュメント：InterSystems IRIS セキュリティ](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GORIENT_ch_security)

- [ビデオ（英語）：Users and Roles in InterSystems IRIS](https://learning.intersystems.com/course/view.php?name=Users%20Roles%20IRIS)


### セキュリティの設定と管理

- [ドキュメント：^SECURITY](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSTU_seccli_security)

- [ドキュメント：サービスの管理](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_manage_services)

    対象：概要説明と「使用可能なサービス」

- [ドキュメント：暗号化データベースの使用法](https://docs.intersystems.com/irislatestj/csp/docbook/Doc.View.cls?KEY=ROARS_encrypt_dbmgmt)

    対象：概要説明と「暗号化データベースの作成」

    参考：[データベースの暗号化手順について](https://jp.community.intersystems.com/node/485826)

- [ドキュメント（クラスリファレンス）：Security.User　Export()](https://docs.intersystems.com/irislatest/csp/documatic/%25CSP.Documatic.cls?&LIBRARY=%25SYS&CLASSNAME=Security.Users#Export)

    参考：[セキュリティ設定のエクスポートとインポートに関するTips](https://jp.community.intersystems.com/node/534526)

### 認証

- [ドキュメント：LDAP and InterSystems IRIS®](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=ROARS_iam_ldap)

- [ドキュメント：2要素認証](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=ROARS_iam_twofactor)

    対象：「2要素認証」

---
## 5. <img src="./assets/icons/5.png" width="70%"/>
システムの健全性を監視し、潜在的な問題を早期に発見する方法を学びます。

- [ドキュメント：システム監視ツール](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCM_monitor#GCM_monitor_tools)

- [ドキュメント：^SystemPerformance を使用したパフォーマンスの監視](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCM_systemperf)

    対象：「^SystemPerformance ユーティリティの実行」

- [ドキュメント:管理ポータルを使用したInterSystemsの監視](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCM_dashboard)

- [ドキュメント：システム・モニタ](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCM_healthmon_sysmon)

- [ドキュメント：データベースの詳細ページ](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_manage_databases_details)


---
## 6. <img src="./assets/icons/6.png" width="70%"/>
プロセス、ロック、ジャーナリングの管理について学習します。

- [ドキュメント：プロセス管理](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSTU_process)

    冒頭の紹介文のみお読みください

- [ドキュメント：ロックの管理](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCOS_locktable)

- [ドキュメント：システム全体での現在のロックの管理](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCOS_locktable_viewall)

    概要説明のみお読みください

    参考
    - [ロックテーブルの使用状況を簡単に確認する方法](https://jp.community.intersystems.com/node/495426)

    - [プログラム内でロック情報を取得する方法](https://jp.community.intersystems.com/node/484976)

    - [アプリケーションでロックタイムアウトエラーが発生する理由](https://jp.community.intersystems.com/node/493701)

- [ドキュメント：タスク・マネージャの使用](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSA_manage_taskmgr)

    参考
    - [プログラミングでタスクスケジュールを登録・参照する方法](https://jp.community.intersystems.com/node/492746)

    - [タスクスケジュールを別環境にコピーする方法](https://jp.community.intersystems.com/node/494331)

    - [タスクの起動でエラーが発生した時にメールで通知する方法](https://jp.community.intersystems.com/node/518651)

- [ドキュメント：ジャーナリングの概要](https://docs.intersystems.com/irislatestj/csp/docbook/Doc.View.cls?KEY=GCDI_journal_overview)


- [ドキュメント：ジャーナリング処理タスク](https://docs.intersystems.com/irislatestj/csp/docbook/Doc.View.cls?KEY=GCDI_journal_tasks)

    参考
    - [ジャーナルファイルの使用量をチェックする方法](ジャーナルファイルの使用量をチェックする方法)

    - [ジャーナルファイルを削除する方法](https://jp.community.intersystems.com/node/501426)

    - [ジャーナルのON／OFFについて、コマンドで操作する方法を教えてください。](https://faq.intersystems.co.jp/csp/faq/result.csp?DocNo=276)

    - [グローバル単位でジャーナルのON/OFF設定する方法](https://jp.community.intersystems.com/node/508706)

    - [ジャーナルの整合性チェックやサマリの表示をコマンドで実行する方法](https://faq.intersystems.co.jp/csp/faq/result.csp?DocNo=582)

    - [ジャーナル圧縮機能について](https://jp.community.intersystems.com/node/537211)

    - [IRISジャーナル（z圧縮済み）をCachéにリストアする方法](https://jp.community.intersystems.com/node/542656)

---
## 7. <img src="./assets/icons/7.png" width="70%"/>
パフォーマンス・メトリクスを確認し、SQL クエリを特定して最適化します。次に、Enterprise Cache Protocol (ECP) がどのようにスケーラビリティを向上させるかを確認します。

### SQLパフォーマンスの最適化
- [ビデオ（英語）：Optimizing Your SQL Queries](https://learning.intersystems.com/course/view.php?id=1013)

    ✅ 記事：[クエリをチューニングする方法](https://jp.community.intersystems.com/node/502256)

- [ドキュメント：SQL パフォーマンスを向上させるためのベスト・プラクティス](https://docs.intersystems.com/irislatestj/csp/docbook/Doc.View.cls?KEY=AGSOB#AGSOB_troubleshoot)


> **英語ビデオもあります**
>
>✅[ビデオ（英語）：Optimizing Your SQL Queries](https://learning.intersystems.com/course/view.php?id=1013)
{: .block-tip}

### ECPを使用したスケーラビリティの実現

- [ドキュメント：分散キャッシュによるユーザ数に応じた水平方向の拡張](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GSCALE_ecp)

- [記事：データプラットフォームとパフォーマンス-パート7 パフォーマンス、スケーラビリティ、可用性のためのECP](https://jp.community.intersystems.com/node/476811)

---
## 8. <img src="./assets/icons/8.png" width="70%"/>
ミラーリング、定期的なバックアップ、ジャーナリングによる高可用性の実装方法を学びます。

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


### ミラーリング

- [ドキュメント：InterSystems IRISミラーリング](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GHA_failover_mirror)

    - ビデオ：ミラーリングを使用したHAおよびDRの構成例(https://www.youtube.com/watch?v=sp5wfKbqHuQ&list=PLzSN_5VbNaxCeC_ibw2l-xneMCwCVf-Or&index=5&t=3s)

{% include youtube-list.html id="sp5wfKbqHuQ" list="PLzSN_5VbNaxCeC_ibw2l-xneMCwCVf-Or&index=5" %}  

- [ドキュメント：ミラーの監視](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GHA_mirror_monitor)

### ジャーナル

- [ドキュメント：ジャーナリングの構成](https://docs.intersystems.com/irislatestj/csp/docbook/Doc.View.cls?KEY=GCDI_journal_config)


---
## 9. <img src="./assets/icons/9.png" width="70%"/>
アップグレード・ガイドおよびリリース・ノートを使用して、InterSystems IRIS をアップグレードします。

- [ドキュメント：アップグレードの概要](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GCI_overview)    

- [InterSystems IRISコンテナのアップグレード](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=ADOCK_iris_upgrading)

- [最新リリースノート(英語)](https://docs.intersystems.com/irislatest/csp/docbook/DocBook.UI.Page.cls?KEY=PAGE_release)

---
## 10. <img src="./assets/icons/10.png" width="70%"/>

エラーの早期発見や問題の迅速なトラブルシューティングに役立つ多くのツールについてご紹介します。
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
## 11. <img src="./assets/icons/11.png" width="70%"/>
あなたのスキルを総動員して、基本的なシステム管理作業を実際にやってみましょう。

- [演習環境（英語ページ）:Performing Common InterSystems IRIS Management Tasks](https://learning.intersystems.com/enrol/index.php?id=1945)

    IRISのインストールをお試しいただけます（Ubuntuを利用）。また、インストール後にデータベースキャッシュサイズとジャーナル設定をいくつか変更します。

---
## 12. 次は？
学習を継続する場合は以下のリソースが最適です。

- [ドキュメント：トラブルシューティングの支援](https://docs.intersystems.com/irislatestj/csp/docbook/DocBook.UI.Page.cls?KEY=GOPS_troubleshoot)
- [記事：「InterSystemsデータプラットフォームのキャパシティプランニングとパフォーマンス」シリーズの索引](https://jp.community.intersystems.com/node/477596)
- [講師付きトレーニング:InterSystems Serverシステム管理1](https://www.intersystems.com/jp/intersystems-server-system-administration/)


- [講師付きトレーニング:InterSystems Serverシステム管理2(セキュリティ管理編)](https://www.intersystems.com/jp/intersystems-server-system-administration-2/)
