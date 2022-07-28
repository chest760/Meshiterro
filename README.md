# Meshiterro

### 作成手順

#### 1 アプリケーションの作成
```
rails new meshiterro
``` 
#### 1.1 トップページの作成 
・homeコントローラーの作成(with topアクション)<br>
```
rails g controller homes to
```
・topをルートページに設定(以下をconfig/routes.rbに追加)
```
root to: "homes#top"
```

#### 1.2 ActiveStorage のインストール
・ActiveStorage の install コマンド実行
```
rails active_storage:install
```
・migrate
```
rails db:migrate
```

#### 1.3 Gemを導入する
・Gemfileに以下のコメントアウトを解除
```
# gem 'image_processing', '~>1.2'
```
・「image_processing」を使える状態にするために以下のコマンドを実行
```
bundle install
```
