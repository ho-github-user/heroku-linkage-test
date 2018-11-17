- 自分用メモ：heroku php deploy用のサンプルプロジェクト(cloneしたもの)
- このリポジトリのmasterにプッシュすると、herokuに自動デプロイされるところまで。
- herokuアカウントつくる
- heroku上でプロジェクト作る(heroku createで簡単につくれる)
- deployの設定で、github connectを許可し、対象のリポジトリを選ぶ
- auto deployみたいなボタンがあるので、押して有効にする
- 基本的にはこれだけで、github - heroku 自動deployできる
- 他にやりたかったこと
  - heroku deploy のslack通知
    - addonの設定が必要らしく、無料だがcredit card登録が必要。一旦見送りした。
  - Travis CIとの連携
  - git push -> ci test run -> heroku deploy の流れがやりたかった
 
# php-getting-started

A barebones PHP app that makes use of the [Silex](http://silex.sensiolabs.org/) web framework, which can easily be deployed to Heroku.

This application supports the [Getting Started with PHP on Heroku](https://devcenter.heroku.com/articles/getting-started-with-php) article - check it out.

## Deploying

Install the [Heroku Toolbelt](https://toolbelt.heroku.com/).

```sh
$ git clone git@github.com:heroku/php-getting-started.git # or clone your own fork
$ cd php-getting-started
$ heroku create
$ git push heroku master
$ heroku open
```

or

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

## Documentation

For more information about using PHP on Heroku, see these Dev Center articles:

- [Getting Started with PHP on Heroku](https://devcenter.heroku.com/articles/getting-started-with-php)
- [PHP on Heroku](https://devcenter.heroku.com/categories/php)
