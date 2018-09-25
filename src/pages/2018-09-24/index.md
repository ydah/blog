---
title: 【Linux】複数コマンドを一行でまとめて実行するセミコロン
date: "2018-09-24"
---

![Koala](./koala.jpg)  

---

## 複数コマンドを一行でまとめて実行するセミコロン

Linuxでコマンドの間に `;` が入っていたら、そこで改行が入っていると思えばよいです。  
`;` は区切り文字として扱われます。

複数のコマンドを一行で実行したいときなどに使えます。  
command1が終了したらcommand2を実行します。

```sh
$ command1; command2
```

### エラーが起こった時の挙動

`;` でコマンドを羅列した場合、command1が成功しても失敗してもcommand2が実行されてしまいます。
つまりエラーがあっても停止はしてくれませんので注意が必要です。