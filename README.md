# FuurinChecker
Simple Japanese notation variation checker for Google Colaboratry

Google Colabotory環境で、テキストファイルの日本語文中から異なる表記（異体字等）をつかっている名詞を出力します。 
spaCyの機能をごく簡単に呼び出すことで、実装してみました。

たとえば、次のような日本語の文章のテキストファイル（input_sampke.txt)を与えると、

> 附属図書館では本の貸出をしています。
> 利用にあたっては付属図書館の規則を確認しましょう。
> 
> 学食のうな丼はおいしいです。
> でも、地元のうなぎ屋の鰻丼のほうが好みかも。
> 
> Googleを大文字化するとGOOGLEになります。

このように結果を返します。

```
附属 付属
うな 鰻
Google GOOGLE
うな丼 鰻丼
```

なお、名称は表記が「揺れると気づく」ということから風鈴=Fuurin Chekerとしてみました。
