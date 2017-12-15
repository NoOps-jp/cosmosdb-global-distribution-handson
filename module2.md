# Module2: Azure Cosmos DBの操作

## 1. サンプルデータの追加

1. データエクスプローラーのCOLLECTIONペインにて、 **Todo**データベース内の **Items**コレクションを展開し、**Documents**をクリックします。

1. **Documents** タブで、**New Document**をクリックします。

1. 以下を参考にJSONドキュメントを編集します。

    ```JSON
    {
        "name": "サンプルデータ１",
        "description": "これは1件目のサンプルデータです。",
        "isComplete": false
    }
    ```

    ```id```はJSONで記述を省略すると自動で採番されます。```name```と```description```の値は任意の文字列を入れて構いません。

1. **Documents** タブで、**Save**アイコンをクリックします。

## 2. データの確認

1. 追加されたデータは、**Documents** タブのリストからidを選択して確認することができます。

    ```_rid```などアンダースコアから始まる項目は、Cosmos DBが内部で管理するデータです。

1. そのままJSONを編集し、**Save**アイコンをクリックすると、データを変更できます。

    管理項目は編集しないようにして下さい。

## Op. Azure Storage Explorer を使う

デスクトップアプリケーションである **Azure Storage Explorer** を使って、Azure Cosmos DBのデータを操作することができます（プレビュー）。Windows、Linux、および MAC バージョンがサポートされています。

* 利用手順: [Azure Cosmos DB を Azure Storage Explorer で管理する (プレビュー)](https://docs.microsoft.com/ja-jp/azure/cosmos-db/tutorial-documentdb-and-mongodb-in-storage-explorer)