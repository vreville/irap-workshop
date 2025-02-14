

## Configuration

https://git-scm.com/book/fr/v2/D%C3%A9marrage-rapide-Param%C3%A9trage-%C3%A0-la-premi%C3%A8re-utilisation-de-Git

    git config --global user.name "Richard Hitier"
    git config --global user.email  rhitier@irap-omp.eu
    git config --list 
    cat ~/.gitconfig


    mkdir ~/tmp/toto && cd ~/tmp/toto
    git init 
    echo hello >> hello.txt 
    git commit -am “init”
    git log
