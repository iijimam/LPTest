---
title: InterSystems IRIS のコンテナとクラウドへの展開
date: 2024-12-01
permalink: DeployingIRISContainerAndCloud.html
layout: post
---

>オリジナル：[Deploying InterSystems IRIS in Containers and the Cloud](https://learning.intersystems.com/enrol/index.php?id=2141)

スケーラブルなデプロイメント戦略を使用して、InterSystems IRIS® データプラットフォームの実装に信頼性を追加できます。

このパスでは、InterSystems IRIS のクラウドおよびコンテナベースのデプロイメントを作成する方法を解説します。

最初にシステムとデプロイメントの仕様概要を説明します。次に、デプロイメント毎の例をご覧いただき、システムに最適なアプローチを確認することができます。

---

[1. <img src="./assets/icons/Container1.png" width="40%"/>](#1-)

[2. <img src="./assets/icons/Container2.png" width="40%"/>](#2-)

[3. <img src="./assets/icons/Container3.png" width="40%"/>](#3-)

[4. <img src="./assets/icons/Container4.png" width="40%"/>](#4-)

---
## 1. <img src="./assets/icons/Container1.png" width="70%"/>

クラウドまたはコンテナへの InterSystems IRIS のデプロイの準備として、システムとデプロイに必要な内容を決定します。

### システム要件
InterSystems IRIS の新規導入を開始する際には、以下のようなシステム要件の詳細な説明を作成します。

- システム・ユーザの数と開発者や管理者などの役割
- 接続する外部システムの数
- 想定されるデータベース・サイズとデータ・フロー量
- サーバーの可用性ニーズ

### デプロイの仕様
次に、いくつかの重要な技術的質問に答えながら、デプロイの仕様を作成します。

- 何台のインスタンスが必要で、どこにデプロイするのか？
- 各インスタンスに必要なデータベースと機能は何か。
- どの程度までデプロイを自動化するか?
- 将来のアップデートはどのように計画しているか？
- インストール時使用するサードパーティソフトウェアがある場合はそれは何ですか？
- 実装ではシャーディングを使用しますか？
- 実装ではミラーリングを使用しますか？

> **英語ページ**
>[Job Aid: Define system requirements and deployment specifications](https://learning.intersystems.com/mod/page/view.php?id=13225)
{: .block-tip}
---
## 2. <img src="./assets/icons/Container2.png" width="70%"/>

InterSystems IRIS をコンテナやクラウドに導入するための戦略をご紹介します。

✅ ビデオ：Dockerコンテナ版InterSystems IRIS data platformの勧め

{% include youtube-list.html id="yY8BLUYp5IA" list="PLzSN_5VbNaxAUiQkx5d22TX0zjx4Mmqhb&index=1" %}

✅ ビデオ：KubernetesでのIRISの運用とそれを支える仕組み

{% include youtube-list.html id="yKX8wB9d2cs" list="PLzSN_5VbNaxC2mfu1cYvn9pfbJRs7xtkk&index=1" %}

> **英語ビデオもあります**
>- [ビデオ（英語）:Tools for Running and Deploying InterSystems Containers](https://learning.intersystems.com/course/view.php?name=ContainerTools1)
>
>    InterSystems IRIS® データ・プラットフォームで利用可能なデプロイメント・ツールについて学ぶことで、ニーズに合ったコンテナ・ベースのシステムを設計することができます。
>
>    このビデオでは
>    - コンテナと Docker の基本を確認します。
>    - InterSystems IRIS 組み込みの 2 つのデプロイ機能、永続的な %SYS と構成のマージについて学びます。
>    - デプロイメント・プラットフォームの利点を紹介します（InterSystems Kubernetes Operator）
>
>    > InterSystems Cloud Manager についてビデオの説明に含まれていますが、バージョン2023.3より deprected となりました。
>
{: .block-tip}

- [ビデオ（英語）：Using Distributed Deployments to Improve Scalability, Compliance, and Availability](https://learning.intersystems.com/course/view.php?name=Distributed%20Deployments)


---
## 3. <img src="./assets/icons/Container3.png" width="70%"/>

- [ビデオ（英語）:Docker Containers and InterSystems IRIS](https://learning.intersystems.com/enrol/index.php?id=888)

    このビデオシリーズでは、Dockerコンテナとその用途を紹介し、InterSystems IRIS®データプラットフォームと組み合わせた場合に、いかに効果的であるかを紹介しています。
    
    また、コンテナが継続的インテグレーション、継続的デプロイメント（CICD）アプローチにどのように適合するかもご理解いただけます。

- Dockerを使用して InterSystems IRIS Community Edition を動かす

    記事：[InterSystemsコンテナレジストリの使い方とコンテナ開始までの流れ（解説ビデオ付き）](https://jp.community.intersystems.com/node/545786)

    {% include youtube-list.html id="HEGWVP0PIfI" list="PLzSN_5VbNaxAUiQkx5d22TX0zjx4Mmqhb&index=2" %}



> **英語のビデオもあります**
>- [ビデオ（英語）:Run InterSystems IRIS Community Edition Using Docker](https://learning.intersystems.com/enrol/index.php?id=1762)
{: .block-tip}

- [体験環境付き演習（英語）：Deploying and Customizing InterSystems IRIS Containers](https://learning.intersystems.com/course/view.php?id=2170)

- [ビデオ（英語）：Automating the Configuration of InterSystems IRIS Instances](https://learning.intersystems.com/course/view.php?id=1624)

    CPFマージ機能により、InterSystems IRIS®データ・プラットフォーム・インスタンスの最終的な状態を簡単かつ宣言的な方法で定義する事ができます。
    
    このビデオでは、CPFマージを利用したクラウドネイティブでGitOpsのようなコンフィギュレーション操作についてご説明します。

    ✅[サンプルコード](https://github.com/intersystems-community/configuration-merge-file-2020.4)：コンテナ化されたデプロイメント用の構成ファイルの使用方法の例がいくつか含まれています。

    - Docker-compose ファイル
    - CPFマージファイル (CPF)
    - 永続的な%SYS
    - グローバル バッファ、ルーチン バッファ、Syslogのエラーログエントリ数、gmheap、locksiz（ロックテーブルサイズ）の自動構成
    - SQL用設定の自動構成
    - ネームスペースとデータベースの自動構成
    - ミラーリングされたデータベースとアービターの自動構成 
    - シャードアーキテクチャの自動構成

---
## 4. <img src="./assets/icons/Container4.png" width="70%"/>

Kubernetes は、コンテナのデプロイ、スケーリング、および管理を自動化するためのオーケストレーション・エンジンです。

InterSystems Kubernetes Operator が InterSystems 固有の機能をどのように追加しているのかを確認し、クラスタをデプロイする演習に挑戦してください。


- [ビデオ（英語）：Kubernetes Overview](https://learning.intersystems.com/enrol/index.php?id=1753)
    
    複数のホストにまたがるコンテナのデプロイをオーケストレーションするためのオープンソースプラットフォームである Kubernetes についてご紹介します。
    
    InterSystems Kubernetes Operator により、InterSystems IRIS®データプラットフォームのユーザは、InterSystems IRISアプリケーションのデプロイメントにおいて Kubernetes メリットを享受することができます。

- [ビデオ（英語）：Deploying and Upgrading InterSystems IRIS with the InterSystems Kubernetes Operator](https://learning.intersystems.com/course/view.php?name=Deploying%20%26%20Upgrading%20IRIS%20with%20Kubernetes%20Operator)

    InterSystems Kubernetes Operator を使用して Kubernetes クラスターを拡張する方法、および InterSystems IRIS® データプラットフォームインスタンスをデプロイ、アップグレード、拡張する方法をご覧ください。

- [体験環境付き演習（英語）：Achieving High Availability with InterSystems IRIS and Kubernetes](https://learning.intersystems.com/enrol/index.php?id=1962)

    KubernetesをInterSystems IRIS®データプラットフォームと組み合わせて使用することで、デプロイメントで高可用性を実現する事ができます。
    
    この演習では、クラスタをデプロイし、災害シナリオをシミュレートし、Kubernetes がどのようにデータ損失とダウンタイムを防止するかを学びます。

ご参考ビデオ：オープンソースだけで IRIS on Kubernetes を動かそう

{% include youtube-list.html id="zMhPuBFl6l4" list="PLzSN_5VbNaxC2mfu1cYvn9pfbJRs7xtkk&index=2" %}