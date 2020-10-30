# Кастомный .vimrc с кучей удобных плагинов

Привет! Я собрал много полезных вещей в одном месте чтобы вы могли кодить в своем любимом виме также удобно как и в любой IDE.

Установка потребует терпения но результат стоит того!

+ [Установка](#Install)


Примеры
=======

<iframe src='//gifs.com/embed/snippets-5QYQAK' frameborder='0' scrolling='no' width='796px' height='454px' style='-webkit-backface-visibility: hidden;-webkit-transform: scale(1);' ></iframe>

##### <a name="Install"></a>

Установка
=========
Начнем:

Для начала тебе потребуется homebrew на личный компьютер используйте эту команду:

    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"

Если вы устанавливаете на компьютер школы то эту:

    curl -fsSL https://rawgit.com/kube/42homebrew/master/install.sh | zsh

После установки homebrew нужно ввести в терминал:
   
    brew install vim cmake go

Эти пакеты необходимы для распаковки и корректной работы плагинов. 
Так ну с homebrew мы разобрались, теперь приступим к установки плагинов для вима, начнем с самого главного - Vundle, просто пропишите это в терминал:

    git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

Как только установите Vundle зайдите в папку репозитории моей сборки и используйте эту команду в терминале:

    ./copy_files.sh

Затем :
    
    vim ~/.vimrc

(могут быть ошибки при входе в вим т.к. плагины не установлены просто жмем энтр)

И установите плагины находясь в открытом .vimrc этой командой:

    :PluginInstall
    
Ждите, установка займет какоето время, не стоит пугатся если установка стоит долго на одном плагине это норм))
Как только увидите в низу с лева заветное слово Done! нажмите q, после чего выйдете с вима.

Теперь нужно распаковать YouCompleteMe, для этого воспользуйтесь этими командами:
    
        cd ~/.vim/bundle/YouCompleteMe
        
        python3 install.py --all
 
Установите хеадер 42 даже если вы устанавливаете на школьный компьютер, лично я устанавливал этот (следуйте гайду по установке) - https://github.com/42Paris/42header

Установите oh-my-zsh используя команду в терминале:

        sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
   
При установке oh-my-zsh меняется конфиг .zshrc поэтому нужно снова зайти в папку с моей сборкой и выполнить команду в терминале:

        ./copy_files.sh
   
Готово!
Осталось перезайти в терминал и наслаждатся удобным вимом :)

Если возникли вопросы или что то пошло не так пишите - мой ник в Intra42 как и в Slack: ctristan, Telegram @nan_deska

















