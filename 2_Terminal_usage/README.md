# Terminal Usage

## Introduce 
終端機（Terminal）是一種命令列介面（Command-Line Interface, CLI），簡單說就是一個<b>提供使用者輸入指令的工具</b>，讓使用者能訪問操作系統，像是文件管理、軟體安裝、系統環境變數設置等功能。

## 使用方式
<kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>T</kbd>

## Common Commands
在介紹常用指令前，可能會有些人在網路上看到別人提供的指令有 <b>"\$"</b> 符號作為開頭，通常那是讓其他人知道這是要輸入在 Terminal 中的指令，但實際輸入指令時是不需要輸入的。

```bash=
user@my_computer_name:~$ ls 
# 實際有效指令只有 ls，並沒有包含 $，複製指令的時候別不小心複製到
```

### Sudo

(Superuser DO) 超級使用者權限。跟以管理員身分執行一樣(可結合其他指令一同使用，請小心使用)

```bash=
user@my_computer_name:~$ sudo
```

### apt-get

用於安裝，更新，升級和刪除任何軟體套件

- **sudo apt-get update**

    更新您的系統有哪些可安裝的軟體套件。

  ```bash=
  sudo apt-get update
  ```

- **sudo apt-get upgrade**

    更新可以升級的軟體套件。

  ```bash=
  sudo apt-get upgrade
  ```

    上述指令會將能更新的軟體套件一併升級，若只想更新特定軟體，可以在後面指定軟體名稱。

  ```
  sudo apt-get upgrade tmux # 只升級 tmux 這個軟體
  ```

- **sudo apt-get install ${package} name you wish to install_**
  安裝指定的軟體，\${package} 請改成你要下載的軟體名稱

  ```
  sudo apt-get install curl # 安裝名為 "curl" 的軟體
  ```
 
### Others common commands
詳細使用範例可以到 reference 提供的網址或日後上網自行查詢
| Command    | Description                |
| :--------- | :------------------------ |
| ls         | 列出目錄的內容 |
| cd         | 切換到不同的目錄 |
| mkdir      | 建立一個新的目錄 |
| cp         | 複製一個檔案或一個目錄 |
| mv         | 用來移動或重新命名一個檔案或目錄 |
| cat        | 顯示一個檔案的內容 |
| grep       | 根據給定的模式對輸出進行排序 |
| chmod      | 更改一個檔案或目錄的權限 |
| ssh        | 遠端連線的一種方式 |
| find       | 搜尋檔案或目錄 |
| history    | 取得先前執行過的命令  |

## reference
1. [25 Must-Know Ubuntu Commands](https://learnubuntu.com/top-ubuntu-commands/)
2. [Basic Ubuntu Commands](https://gist.github.com/TechRancher/770a7a2ab7f0edb687e8048e538122e3)