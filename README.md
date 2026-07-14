[README.md](https://github.com/user-attachments/files/29995755/README.md)
# 完全版：クラシックギター楽譜難易度評価調査

## GitHubへアップロードするもの
- index.html
- instructions.pdf
- pdf/edition1 ～ pdf/edition4 内の楽譜PDF

`admin_only` フォルダはアップロードしません。

## 楽譜PDFの名前
各版のフォルダに `01.pdf` から `10.pdf` を置きます。

## Apps Script
1. Googleスプレッドシートで「拡張機能 → Apps Script」を開く。
2. Code.gsを全置換する。
3. Google Driveへ大学指定の transfer.xlsx をアップロードする。
4. Drive URLの `/d/` と次の `/` の間のファイルIDを、Code.gsの `PAYMENT_TEMPLATE_FILE_ID` に貼る。
5. 「デプロイ → デプロイを管理 → 編集 → 新しいバージョン」で更新する。
6. 実行ユーザーは自分、アクセスできるユーザーは全員。

## 保存先
- participants：氏名・メール・属性
- responses：4版の評価（参加者1名につき4行）
- Google Driveの guitar_survey_payment_files：記入済みExcel

## 説明書
同梱の instructions.pdf は動作確認用のたたき台です。倫理審査で承認された正式な研究説明書に差し替えてください。ファイル名は instructions.pdf のままにします。

## 必須テスト
1. 説明書が表示される。
2. 属性入力後に4版を評価できる。
3. 未入力の曲があると次へ進めない。
4. 支払いExcelをダウンロードできる。
5. 記入済みExcelを送信できる。
6. participantsに1行、responsesに4行、Driveに1ファイル保存される。

## 注意
GitHub Pages上のファイルは公開されます。楽譜はパブリックドメインで、かつ使用する版の権利状態も確認してください。
