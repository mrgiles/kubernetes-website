---
title: イミュータブルインフラストラクチャ
id: immutable-infrastructure
date: 2024-03-25
full_link:
short_description: >
  イミュータブルインフラストラクチャはデプロイ後に変更できないコンピューターインフラストラクチャ(仮想マシン、コンテナ、ネットワークアプライアンス)を指します。
aka: 
tags:
- architecture
---
イミュータブルインフラストラクチャはデプロイ後に変更できないコンピューターインフラストラクチャ(仮想マシン、コンテナ、ネットワークアプライアンス)を指します。
<!--more-->

イミュータビリティ(不変性)は、不正な変更に対して自動で上書きする処理や、そもそも変更を許可しないシステムによって強制的に維持されます。

{{< glossary_tooltip text="コンテナ" term_id="container">}}はイミュータブルインフラストラクチャの良い例です。
コンテナへの永続的な変更は、新たなバージョンでコンテナを作成するか、既存のコンテナをイメージから再作成する方法しかないためです。

不正な変更を阻止または特定することで、イミュータブルインフラストラクチャはセキュリティリスクの特定と軽減を容易にします。
このようなシステムの運用は管理者が想定できるため、より簡単になります。
結局のところ、彼らは誰もミスや伝え忘れた変更がないことを知っています。
イミュータブルインフラストラクチャは、インフラストラクチャの作成に必要なすべての自動化をバージョン管理(Gitなど)に保存する、Infrastructure as Codeと密接に関係しています。
このイミュータビリティとバージョン管理の組み合わせは、システムに対するすべての許可された変更の永続性のある監査ログが存在することを意味します。