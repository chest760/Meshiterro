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
