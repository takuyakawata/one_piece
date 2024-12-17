# one_piece

# 使用技術

## プログラミング言語
- Kotlin

## フレームワーク
- Spring Boot: サーバーサイドのフレームワークとして使用
- Casbin: アクセス制御のためのライブラリ
- Jooq: 型安全なSQLクエリ生成のためのライブラリ

## ツールやサービス
- AWS: クラウドインフラストラクチャ
- Docker: コンテナ化による開発環境の構築
- MySQL: データベース
- Gradle: プロジェクトのビルドツール

## セットアップ手順


### Dockerコンテナのセットアップ
#### MySQL コンテナ
- `docker-compose.yml` で MySQL と Casbin を設定。
- MySQLコンテナは、データ永続化のためにボリュームを使用。

#### Casbin コンテナ
- Casbin は、API サーバー内でアクセス制御を実装。
- Go で作成した Casbin アプリケーションをコンテナ内で実行。

### 必要な依存関係のインストール
```bash
./gradlew build
```
### アプリケーションの起動
```bash
./gradlew bootRun
```
