# sample-gas


## 最初にやること
1. .clasprc.json を作成
  - `clasp login --no-localhost`
1. GoogleAppsScript API の許可
  - https://script.google.com/home/usersettings
1. プロジェクト作成
  - Google Drive上でフォルダを作成しておく（自分が認識できれば名前はなんでも良い）
  - `clasp create --title clasp-sample-project --parentId {GoogleDriveのフォルダID} --rootDir ./src`
1. デプロイ
  - `clasp deploy`    # 検証用
  - `clasp deploy`    # 本番用
  - 以降は `yarn deploy-production`
1. 動作確認
  - `curl -H "Content-Type: application/json" -L https://script.google.com/macros/s/<clasp deploy>/exec`
  - `curl -H "Content-Type: application/json" -L https://script.google.com/macros/s/<clasp deploy>/exec -d {}`
