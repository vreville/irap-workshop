
## Supports:


https://www.canva.com/design/DAGfErt9Phc/s-wMOeFwsPFuiE6Q7DoT3A/view

## Configuration

https://git-scm.com/book/fr/v2/D%C3%A9marrage-rapide-Param%C3%A9trage-%C3%A0-la-premi%C3%A8re-utilisation-de-Git


### basic config

    git config --global user.name "Richard Hitier"
    git config --global user.email  rhitier@irap-omp.eu
    git config --list 
    cat ~/.gitconfig



check 

    mkdir ~/tmp/toto && cd ~/tmp/toto
    git init  # check .git/
    echo hello >> hello.txt 
    git add hello.txt
    git commit -am “init”
    git log


### bash+zsh

https://git-scm.com/book/fr/v2/Annexe-A:-Git-dans-d%e2%80%99autres-environnements-Git-dans-Bash


https://github.com/git/git/tree/master/contrib/completion

    wget https://github.com/git/git/blob/master/contrib/completion/git-prompt.sh  ~/
    wget https://github.com/git/git/blob/master/contrib/completion/git-completion.bash  ~/
    . ~/git-prompt.sh
    . ~/git-completion.bash
    export GIT_PS1_SHOWCOLORHINTS=1
    

    # set forever
    cat >> ~/.bashrc  << .END
    . ~/git-prompt.sh
    . ~/git-completion.bash
    export GIT_PS1_SHOWCOLORHINTS=1
    .END



### More configuration

    git config --global alias.l 'log --oneline'
    git config --global alias.co checkout
    git config --global alias.ci commit
    git config --global alias.s 'status -suno'




    git config alias.l 'log --graph --pretty="format:%C(yellow)%h%Cblue%d%Creset %s %C(white) %an, %ar%Creset"'

