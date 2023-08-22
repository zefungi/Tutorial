# Anaconda Installation

## STEP_1. 到官網下載對應版本

[Free Download | Anaconda](https://www.anaconda.com/download)

![Untitled](image/Untitled.png)

若是 ubuntu 版本，下載下來應為 .sh 檔案（ex. Anaconda3-2023.03-1-Linux-x86_64.sh）

## STEP_2. 到下載資料夾執行anaconda 安裝腳本

```bash
cd ~/Downloads
sh Anaconda3-2023.03-1-Linux-x86_64.sh 
#檔名不一定跟範例相同
```

執行過程中一直按 Enter，**直到它向你確認 yes/no後，記得要輸入 yes**

![Untitled](image/Untitled%201.png)

![Untitled](image/Untitled%202.png)

輸入完後會問你安裝路徑，若沒有特別需求，可按 Enter 跳過
（Anaconda 會以家目錄當作預設路徑  ex. ~/anaconda3 or /home/${USER}/anaconda3）

![Untitled](image/Untitled%203.png)

最後會在向你詢問，是否每次開啟 Terminal 時，自動開啟 base 的 conda 環境，可以輸入 yes

## BASH 針對 anaconda 相關指令自動補字
[conda-bash-completion](https://github.com/tartansandal/conda-bash-completion)