# Installation for Ubuntu

###### tags: `ubuntu`, `vim`, `vscode`

## 文字編輯器：vim, vscode, ...
### vim
- **Installation**
    ```bash=
    sudo apt-get install vim
    ```
- **Usage**
    
    在終端機輸入 vim 後即可進入 vim 文字編輯器的畫面。vim 主要分為 insert mode, command mode，不同模式可執行不同指令。
    
    - Insert Mode 

        按下 <kbd>i</kbd> 後即可開始修改檔案內容，若要結束 insert mode，則按 <kbd>Esc</kbd>
    
    - Command Mode
        不論是剛進 vim 畫面，或是按下 <kbd>Esc</kbd>，皆為 Command Mode。

        | Command | Description|
        |:-|:-|
        |:w|save change|
        |:q|quit without saving|
        |:wq|quit and save|
        |:q!|force quit|

    更多詳細內容可上 reference 的 Vim cheatsheet 網址查詢

- **reference**
    1. [開始在 Vim 裡打字-高見龍](https://www.youtube.com/watch?v=uC4JGhrqLng&ab_channel=%E9%AB%98%E8%A6%8B%E9%BE%8D)
    2. [Basic Vim commands - For getting started](https://coderwall.com/p/adv71w/basic-vim-commands-for-getting-started)
    3. [Vim cheatsheet](https://devhints.io/vim)

### vscode 
[官網下載連結](https://code.visualstudio.com/)


## Terminal 管理工具：tmux
- **Installation**
    ```bash=
    sudo apt-get install tmux
    ```
- **Command Mode**
    先按下 <kbd>Ctrl</kbd> + <kbd>b</kbd>進入 command mode後，再接者按以下對應的符號

    | Command | Description|
    |:-|:-  |
    |%| 垂直分割畫面 |
    |"| 水平分割畫面 |
    |c| 生成新的視窗(bash) |
    |n| 移動到下一個視窗(bash) |
    |${number}| 移動到特定號碼的視窗(bash) |

    更多詳細內容可上 reference 裡的 tmux-cheatsheet 查詢

- **reference**
    1. [tmux-cheatsheet.markdown](https://gist.github.com/MohamedAlaa/2961058)

## 分散式版本控制系統：git 
- **Installation**
    ```bash=
    sudo apt-get install git
    ```

- **Common Commands**
    | Command | Description|
    |:-|:-  |
    | git init | initialize a git root here |
    | git add | add current changes to temp |
    | git commit -m "${Description}" | commit temp into local git dir with message |
    | git push | upload local git dir to remote git dir |
    | git pull | download remote git dir to local git dir |
    | git branch | show branch info |
    | git log | show log of commit and HEAD |
    | git status | show status of current working tree

- **reference**
1. [連猴子都能懂的 Git 入門指令](https://backlog.com/git-tutorial/tw/intro/intro1_1.html)
2. [Git Document](https://git-scm.com/doc)

