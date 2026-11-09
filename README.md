# validation-app-practice

## 概要
COACHTECH 教材 Tutorial 9-6「バリデーション ハンズオン演習」で作成した成果物です。
ユーザー登録画面を作成しました。

## 使用技術
- PHP 8.x
- Laravel 10.x
- FormRequest / バリデーションルール
（**他に使ったものがあれば追記してください**）

## 学んだこと
- バリデーションルールの記述方法。（required, email, unique, min）
- コントローラーで作成したフォームリクエストを読み込む方法
- エラーメッセージの日本語表示方法

## 詰まったポイント
- コントローラーにAuth::login($user)を書いた方がいいかな？と思い書いてみましたがエラーが出たので削除しました。

## 開発の工夫
- UserController.phpの public function store(StoreUserRequest $request)　のメソッドは模範解答のようにすっきりと短く書く方がいいと思いますが、あとから見返したときにパスワードがどのように処理されているかがわかりやすいので１つづつ記述しました。

## 動作確認
（**どうやって動かして確認するかを記載してください**）
- http://localhost/register　へアクセスして正しく動作するか確認。
- 全ての項目を入力して登録を押したときの処理が完了したか。
- 何も入力せずに登録ボタンを押したときにエラーが表示されるか。
- 正しくない入力方法をそれぞれ試してみてエラーが表示されるか。
- <img width="1920" height="869" alt="ユーザー登録" src="https://github.com/user-attachments/assets/89c015ce-230e-4dbd-aa7d-d98a18273ac1" />
