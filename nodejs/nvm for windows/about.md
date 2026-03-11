# NVM for Windows
## 概要
- windows環境でnodejsのバージョン管理を楽に行うためのアプリ
- ターミナルから実行可能
## インストール手順
1. [公式リポジトリ](https://github.com/coreybutler/nvm-windows)のリリース assetsからダウンロードする(最新版を推奨)
2. nvm-setup.exeを実行しインストールを行う
   - 基本的にnextを押していくだけでok
3. インストール後power shell, コマンドプロンプトを起動する
4. 以下を入力,実行し正常にインストールされているかを確認する
   ```shell
   nvm
   ```
   - 正常に実行できない場合は再インストールや,pcの再起動を行う

## 使用方法
- 公式のreadmeを参照(そちらのほうが正確です)
- 本家nvmと基本的に同じです
- ターミナルから操作を行う
### インストール可能なバージョンを表示する
```shell
nvm list available
```
- ここからバージョンを指定してインストールする
### 指定したバージョンをインストールする
```shell
nvm install version
```
- versionにはlistの値をそのまま使用する
- またメジャーバージョンのみの指定で該当バージョンの最新版をインストールする?
   ```shell
   # メジャーバージョン25の最新版をインストールする
   # 2026/3/19現在->25.8.1
   nvm install 25
   ```

### インストール済みのバージョンを表示する
```shell
nvm list
# もしくは
nvm list installed
```

### インストールしたバージョンを使用する
```shell
nvm use version
```
- versionにはlistの値をそのまま使用する
- installと同様メジャーバージョンのみの指定でも可能
- 実行後、プロンプトの許可が必要(ウィンドウが出ます)
- **node -v**でバージョンが切り替わっているかを確認する

### インストールしたバージョンを削除する
```shell
nvm uninstall version
```
- versionにはlistの値をそのまま使用する

## 参考
- [Repository](https://github.com/coreybutler/nvm-windows)

## 更新日時
- 2026/3/19
  - 基本的な使用方法を追加
