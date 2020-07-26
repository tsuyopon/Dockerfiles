# 概要
golangとvimを利用するための環境構築について

以下の環境を用意するためのレシピです。
- golang
- vimでsyntax onが有効となる
- 定義元へ行ったり、戻ったりすることができる。

# 詳細 

以下のimageを使います。
- https://hub.docker.com/r/mbrt/golang-vim-dev/

上のドキュメントに記載の通り
```
cd your/go/workspace
docker run --rm -tiv `pwd`:/go mbrt/golang-vim-dev
```

引数なしでvimを開きます。
```
$ vim
```

上記で開いたら、以下のコマンドでインストールが完了するのを待ちます(しばらく待ちます)
```
:GoInstallBinaries
```

続いて定義元へ遷移したら、元の場所に戻るには
- https://github.com/fatih/vim-go-tutorial#go-to-definition

```
定義元に遷移する:    Ctrl + ]   又は   gd
前の場所に戻る:      Ctrl + t
```



