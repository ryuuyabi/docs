## vpc

例えば、オンプレ環境でWebアプリ(3層アーキテクチャ)と社内システムを運用するために、以下のようなネットワークを構築していたとします。

### メリット
* 通信経路を絞って監視・アクセス制御を行うことで、セキュリティを向上させる
* 通信経路を明示的に制御してロードバランサ等でスケールアウトすることで、性能を担保できる
* 通信経路を明示的に複数確保することで、可用性を向上させる事ができる
* システム内のサービスを整理して一括管理する事で、運用・保守性を向上させる事ができる
* IaCサービスと組み合わせることで、移行性を向上させる事ができる

###### ※ ロードバランサとは？ 複数のサーバに負荷を分散させる装置
###### ※ スケールアウトとは？ システムを構築するサーバーの台数を増やし、分散処理で運用を安定させ、処理能力や可用性を高める
###### ※ IaCサービスとは？ 手動のプロセスや設定の代わりに、コードを使用してインフラストラクチャの管理とプロビジョニングを行うこと

### EC2との違い
