---
page_type: Sample
languages: 
- Japanese
products:
- Power Apps and Power Automate
description: "Power Platformを利用した職域接種予約アプリテンプレート"
urlFragment: "NA"
---

# Official Microsoft Sample - 職域接種予約アプリテンプレート
職域接種予約アプリテンプレートは、新型コロナウイルスワクチン職域接種を申請した企業において、従業員やその家族のワクチン接種予約を管理をする目的で作成されました。このソリューションには、従業員向けのワクチン接種予約アプリ、そして管理者向けの会場や予約枠および当日の受付管理ができるアプリの２つのテンプレートが含まれています。

アプリケーションの利用の概要としては、下記を想定しています。

・管理者は、接種会場の情報と予約可能枠を登録する。

・従業員は、モバイルアプリやPCを使って基本情報を登録し、ワクチン接種希望日程を予約する。

・現場担当者は、管理者用アプリの当日受付・記録機能を使って、従業員の接種状況を記録する。

上記により、職域接種に必要なデータをリアルタイムに管理し、円滑なワクチン接種をサポートします。
![vrapp3](https://user-images.githubusercontent.com/10231266/124684380-f4d17700-df09-11eb-8579-5636ce1e2200.png)


## コンテンツ
本レポジトリには下記のコンテンツが含まれています。

| File/folder                     　　　　　| Description                                              |
|------------------------------------------|----------------------------------------------------------|
| `workplace_vaccination_1_0_0_12.zip`   　　　　　|Power Apps Unmanaged Solution File                        |
| `workplace_vaccination_security_role_1_0_0_1.zip`   　　　　　|Power Apps Unmanaged Solution File                        |
| `職域接種予約アプリ導入手順書.pdf`                              | 導入手順書                                        |
| `README.md`                              | This README file.                                        |
| `LICENSE`                                | The license for the sample.                              |

## 前提条件

本サンプルは、Microsoft Power Apps上で動作します。
そのため、必要なライセンスもしくは評価環境のテナントを取得し評価を行っていただく必要があります。
本サンプルはDataverse for Teams、またはDataverseどちらかの環境を利用をして展開をします。
Dataverse for Teamsで展開する場合、一部機能制限があります為、必要な機能や要件に応じて、適切なライセンスをご用意下さい。（本テンプレートにおける機能差は導入手順書に記載）

[Dataverse for TeamsとDataverseの機能比較](https://docs.microsoft.com/ja-jp/powerapps/teams/data-platform-compare)

## セットアップ

本サンプルでは、Power Apps アプリのセットアップが必要になります。
Zipファイルをアンマネージドソリューションとして登録しています。こちらのアンマネージソリューションをソリューションのインポートでPower Appsの環境に登録をしてご利用ください。
詳細なセットアップ手順は同梱の導入手順書をご参照下さい。

## サンプルの実行

サンプルの実行については、ソリューションファイルをインポート後、一般的なPower Apps のアプリケーションと同様に利用を行う事が可能です。
Dataverse for Teamsに展開した場合は、Teams上でのみ実行が可能となります。

## 構成内容
本テンプレートは下記の要素にて構成されています。

Power Apps ソリューションファイル  
Power Apps ソリューションファイルには次の内容が含まれています。
 - テーブル
 - キャンバスアプリ（利用者用、管理者用）
 - モデル駆動型アプリ（Dataverseに展開時のみ利用可能）
 - フロー
 - その他構成ファイル

## 展開・利用に必要な項目
本テンプレートを展開・利用するにはDataverse for Teamsを利用できるMicrosoft Teamsのライセンス、もしくはDataverseが利用できるPower Appsライセンスが必要です。詳しくは下記をご参照下さい。  
https://powerapps.microsoft.com/ja-jp/pricing/

[Dataverse for TeamsとDataverseの機能比較](https://docs.microsoft.com/ja-jp/powerapps/teams/data-platform-compare)

## 必要なPower Platformの環境
本ソリューションは、Microsoft Teamsライセンスに包含される Dataverse for Teams環境、もしくはPower Appsの有償ライセンスに含まれるDataverse環境へ展開が可能です。

## 準備されている言語
本テンプレートは日本語で準備されており、日本語にのみ対応します。

## 主な機能
主な機能は、下記のとおりです。

職域接種予約アプリ  

職域接種予約アプリは、職域接種を実施する企業の従業員がワクチン接種を予約するためのアプリケーションです。
本アプリケーションの利用は、スマートフォン、タブレット、PCいずれかのデバイスから、配布されたアカウントにてサインインすることにより利用することができます。（Dataverse for Teamsの場合は各デバイスのTeams上から利用）
利用できる主な機能は、ユーザー登録（従業員自身、もしくは家族や社外の方の代理登録）、一回目および二回目のワクチン接種予約、予約確認、予約キャンセル、問い合わせ機能です。
![vrapp](https://user-images.githubusercontent.com/10231266/124683949-285fd180-df09-11eb-84b9-6076ab8a5f29.png)


職域接種管理者用アプリ（タブレット版）  

職域接種管理者用アプリは、職域接種の管理者や接種担当者が接種会場や予約可能枠、接種記録を管理するためのアプリケーションです。
本アプリケーションの利用は、タブレットもしくはPCを想定しています。配布された管理者用アカウントにてサインインすることにより利用することが可能です。
（Dataverse for Teamsの場合は各デバイスのTeams上から利用）
利用できる主な機能は、接種会場の登録、予約可能枠の登録・管理、および当日のワクチン接種受付・記録機能です。
![vrapp2](https://user-images.githubusercontent.com/10231266/124683966-31e93980-df09-11eb-8e1e-65be77e3d1bb.png)


## FAQ
 - Q.内容や機能をカスタマイズすることは可能ですか？
   - A.可能です。
 - Q.サポートはありますか？
    - A.いいえ、ありません。サンプルとしての提供になりますので、ご利用者様の判断にてご利用ください。
 - Q.Dataverse版を評価版にて利用することができますか？
    - A.Power Apps及びPower Automateは、双方とも30日の無償評価版があります。評価版にてご利用、機能の確認を行う事が可能です。


## Contributing
## 免責事項
本テンプレートはサンプルであり、Microsoft Power Appsにおいて、参考情報の提供等の目的で公開されています。本テンプートおよび関連サービスは、恒久的なアプリケーション使用を意図したものではありません。日本マイクロソフトはそのような目的で本テンプレートおよび関連サービスを使用するライセンスや権利を本テンプレート利用組織に付与していません。 本テンプレートおよび関連サービスは、各企業のニーズを全て含めるように設計されたものではなく、そのような用途で使用されるものではありません。実際の利用や必要な追加のカスタマイズは別途導入支援パートナーに確認・依頼してください。 本テンプレートおよび関連サービスのいかなる使用においても、利用者がすべてリスクと責任を負うものとします。また、実装した本テンプレートおよび関連マイクロソフト サービスの使用に関して、適切な警告や情報をエンドユーザーに提供することについても、利用者が責任を負うものとします。 本テンプレートは、日本国内での使用のみを目的とし、欠陥などがある可能性を含んだままの状態で提供されており、いかなる種類の保証も適用されません。

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
