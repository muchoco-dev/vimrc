### 必要なパッケージが入っているか確認(なければインストール sudo yum install )

    $ yum list installed | grep mercurial
    $ yum list installed | grep ncurses-devel
    $ yum list installed | grep make
    $ yum list installed | grep gcc

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
    $ mv vimrc/.vimrc .
    $ rm -r vimrc/

### vim実行

    $ vim
