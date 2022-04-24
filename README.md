# laravel-9

git cloneしてからやること

- コンテナ起動
  - docker compose up -d
- appコンテナに入る
  - docker compose exec app bash
- 以下のフォルダに書き込み権限付与
  - docker compose exec app bash
- vendor ディレクトリへライブラリ群をインストール
  - composer install
- .envがないから.env.exampleをコピーして、.envファイルを作成する
  - cp .env.example .env
  - db情報とかも適宜修正する
- .env に APP_KEY= の値がないと出るから以下のコマンド実施
  - php artisan key:generate
  - php artisan storage:link
- migrationできるか確認
  - php artisan migrate

- 片付け
  - docker compose down --rmi all --volumes --remove-orphans
# scraping
