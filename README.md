# my-azure
<!--  Change title and content as needed -->

# Usage 

## Workflows

### Deploy Resource Group
特定のテナントにリソースグループを作成します。このワークフローは、手動実行のみをサポートします。  
以下のパラメータを入力してください。

|Parameter|Description|Notes|
|-|-|-|
|LOCATION|Enter location of resource group|リソースグループを作成するロケーションを指定します|
|SERVICE_NAME|Enter service name|リソースの識別に使用するサービス名を指定します<br>これはタグにも指定されます|
|ENV_NAME|Enter environment name|環境名を指定します|
|USER_NAME|Enter user name to assign to tag|タグに指定されるユーザ名を指定します|

また、このワークフローを実行する場合は、事前に以下のGitHubシークレットを作成してください。

|Secrets|Notes|
|-|-|
|AZURE_CLIENT_ID|アプリケーションID|
|AZURE_TENANT_ID|テナントID|
|AZURE_SUBSCRIPTION_ID|リソースグループをデプロイするサブスクリプションのID|
|AZURE_USER_OBJECT_ID_001|リソースグループに対するロールを割り当てるユーザのオブジェクトID|

## Author
- **Jun Kato**
    - GitHub : [a7p11t](https://github.com/a7p11t)

## License
This project is released under the Unlicense,
see the [UNLICENSE.md](UNLICENSE.md) file for details.
