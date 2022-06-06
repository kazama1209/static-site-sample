# static-site-sample

Vercel に静的 Web サイトをホスティングしたい（単純に html ファイルと css ファイルを突っ込む形式） → ルーティングはどうすれば良い？（Next.js とかなら適当にやれば良いけど上記の場合はどうすれば良いかわからん）→ ルート直下に vercel.json を作成して

```json
{
  "cleanUrls": true
}
```

を記述すれば OK（例えば、/sp というパスにアクセスすると、sp.html が提供される）

https://vercel.com/docs/project-configuration#project-configuration/clean-urls
