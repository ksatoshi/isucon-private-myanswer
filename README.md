## 修正前
```json
{"pass":true,"score":1017,"success":1055,"fail":6,"messages":["リクエストがタイムアウトしました (POST /login)","リクエストがタイムアウトしました (POST /register)"]}
```

## 修正後
```json
{"pass":true,"score":1290,"success":1305,"fail":5,"messages":["リクエストがタイムアウトしました (GET /logout)","リクエストがタイムアウトしました (POST /login)","リクエストがタイムアウトしました (POST /register)"]}
```

## 総括
今回は主にDBや画像周りの改修を行った。最終的なスコアは270点ほど向上しているため効果があったと考えられる。しかし、パフォーマンスプロファイラーなどを使用し、改善点を見つけ改善したわけではなくある種の勘に従って修正を行ったため劇的な改善結果を得ることはできなかった。  
今回反省すべき点としては、客観的なデータに基づいて改善個所を発見できなかったことだろう。よって、次このような機会があればパフォーマンスプロファイラーを使用しながら最適化を行っていきたいと思う。
