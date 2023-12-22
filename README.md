### コードのREADME

#### 1. 目的

このコードは、Google Colab 上で Google スプレッドシートと Google Drive を連携させ、特定のウェブサイトから情報をスクレイピングして取得し、それを Google スプレッドシートに記録し、また画像を Google Drive に保存する目的で作成しました。

#### 2. 使っているライブラリ

以下のライブラリを使用しています：

- `requests`: ウェブページからデータを取得するためのライブラリ
- `gspread`: Google スプレッドシートへのアクセスを可能にするライブラリ
- `BeautifulSoup`: HTML 解析のためのライブラリ
- `oauth2client.service_account`, `google.oauth2.service_account`, `google.oauth2`: Google API への認証のためのライブラリ
- `PIL`: 画像の取得・保存のためのライブラリ
- `io`: バイトストリームを扱うためのライブラリ
- `os`: ファイルおよびディレクトリの操作のためのライブラリ
- `googleapiclient.http.MediaFileUpload`: Google Drive へのファイルアップロードのためのライブラリ
- `googleapiclient.discovery.build`: Google API へのアクセスを可能にするライブラリ

#### 3. 実行手順

1. Google スプレッドシートと Google Drive にアクセスできるサービスアカウントを作成し、キーを JSON ファイルとしてダウンロードします。
2. ダウンロードした JSON ファイルのパスを `SP_CREDENTIAL_FILE` に設定します。
3. Google スプレッドシートと Google Drive へのアクセス権限を `SP_COPE` に適切に設定します。
4. 画像を保存する Google Drive のフォルダの ID を `target_folder_id` に設定します。
5. スクレイピング対象のウェブサイトの URL を `url` に設定します。
6. コードを実行します。
