## 村上友哉の LaTeX テンプレート置き場

ここは、私村上が私的に作成した LaTeX のテンプレートの保管庫です。

* [記事テンプレート](https://github.com/YuyaMurakamiMath/My_TeX_template/blob/main/%E8%A8%98%E4%BA%8B%E3%83%86%E3%83%B3%E3%83%97%E3%83%AC%E3%83%BC%E3%83%88.pdf)
* [カラフルな記事テンプレート](https://github.com/YuyaMurakamiMath/My_TeX_template/blob/main/%E3%82%AB%E3%83%A9%E3%83%95%E3%83%AB%E3%81%AA%E8%A8%98%E4%BA%8B%E3%83%86%E3%83%B3%E3%83%97%E3%83%AC%E3%83%BC%E3%83%88.pdf)
* [論文テンプレート](https://github.com/YuyaMurakamiMath/My_TeX_template/blob/main/%E8%AB%96%E6%96%87%E3%83%86%E3%83%B3%E3%83%97%E3%83%AC%E3%83%BC%E3%83%88.pdf)

の3つのテンプレートを置いています。

便利なコマンドを豊富に準備し、よく必要になるパッケージをまとめて導入しています。
また、出来る限り整理してあるので、メンテナンスやカスタマイズもやりやすくなっています。
良ければ使ってみてください。

## このテンプレートで出来ること

* ℤ と書くのにいちいち `\mathbb{Z}` と書かずとも、単に `\Z` と書くだけで良くなる
* 他にも行列、色々な括弧、様々な記号、例えば $\mathrm{Ker}, \mathrm{Hom}, \mathrm{GL}_2(\mathbb{R})$ などを短く、そしてTeXの文法として正確に書ける
* TeX

## 注意点

### sty ファイルの使いかた

以下の sty ファイルを利用できます。

* 
* [mycommand.sty](https://github.com/YuyaMurakamiMath/My_TeX_template/blob/main/mycommand.sty): コマンドを楽に入力する
* [mytheorem.sty](https://github.com/YuyaMurakamiMath/My_TeX_template/blob/main/mytheorem.sty): 日本語での定理環境

ここの sty ファイルを利用したいときや tex ファイルをコンパイルしたいときは、同梱されている sty ファイルに対し
* テキストエディタで開き、内容をプリアンプルにコピペする
* tex ファイルと同じフォルダに置く
* （W32TeX の場合）「C:\w32tex\share\texmf-local\tex\(好きなファイル名)」に置く。\share 以下のフォルダが存在しない場合は新しく作成する

のいずれかを行ってください。

自作 sty ファイルで読み込んでいる一部のパッケージ（bbm, bbold, listings, plistings）は、 TeX をインストールする際にデフォルトでインストールされていない可能性があるので、 その場合は別途インストールしてください。
これらのパッケージの sty ファイルの置き場所も「C:\w32tex\share\texmf-local\tex\(好きなファイル名)」です。

### LuaLaTeXを使ってください

ここの tex ファイルは全て **LuaLaTeX でのコンパイルを想定**しています。
日本で主流の upLaTeX + dvipdfmx によるコンパイルは想定していません。
upLaTeX + dvipdfmx でコンパイルできる tex ファイルの作成は、必要な修正が多いことと、 LuaLaTeX を使っている自分には必要ないことから断念しました。
すみません。

私の意見としては、ぜひLuaLaTeXを使ってみてほしいと思っています。
コンパイルが遅いという欠点はあるものの、日本語の文書をLaTeXで作成するのには upLaTeX + dvipdfmx よりも便利だと思います。
具体的には、次のようなメリットがあります。
* 

なお、以下の sty ファイルは upLaTeX + dvipdfmx でも利用できます:
* [mycommand.sty](https://github.com/YuyaMurakamiMath/My_TeX_template/blob/main/mycommand.sty): コマンドを楽に入力する
* [mytheorem.sty](https://github.com/YuyaMurakamiMath/My_TeX_template/blob/main/mytheorem.sty): 日本語での定理環境

### physics パッケージとは非互換

physics パッケージや physics2 パッケージとは互換性がありません。
頑張ってはみたのですが無理でした。
なお、physics パッケージはエラーが多いようなので導入はやめた方が良いかもしれません。

### 免責事項

筆者は TeX をきちんと理解しておらず、誤りが含まれる可能性が多々ありますのでご注意ください
（誤りを見つけた際にはお手数ですがご指摘頂けると大変ありがたく思います）。

また筆者は数学畑（特に整数論）の人間です。 異なる分野の慣習に起因する作法の違いもあると思いますのでご注意ください。
