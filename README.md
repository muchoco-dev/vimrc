### 必要なパッケージが入っているか確認

#### CentOS

    $ dnf list installed | grep mercurial
    $ dnf list installed | grep ncurses-devel
    $ dnf list installed | grep make
    $ dnf list installed | grep gcc

なければインストール sudo dnf install {パッケージ名}

#### Ubuntu

```
$ apt list --installed | grep mercurial
$ apt list --installed | grep ncurses-devel
$ apt list --installed | grep make
$ apt list --installed | grep gcc
```

なければインストール sudo apt install {パッケージ名}

### 7.4以上のvimが入っていることを確認

    $ vim --version

### カラースキーム用のフォルダがなければ作成
    
    $ mkdir ~/.vim
    $ cd ~/.vim
    $ mkdir colors

### カラースキームファイルを取得
    
    $ git clone https://github.com/w0ng/vim-hybrid
    $ mv vim-hybrid/colors/hybrid.vim ~/.vim/colors/

### .vimrcファイルを取得して、ホームディレクトリに置く
    
    $ git clone https://github.com/muchoco-dev/vimrc.git
    $ mv vimrc/.vimrc ~
    $ rm -r vimrc/

### vim実行

    $ vim
