# File Type

## sh (shell script)

shell script (.sh) 這種類型的檔案，簡單說就是一個腳本檔，你可以把原先要在終端機輸入的多筆指令一併寫進其中，這樣就可以執行單一腳本就跑完自己希望在終端機處理的所有事情。

若想要深入了解其運作的概念可以到 Reference 裡或是自行上網查詢。

<b>How to run .sh file</b>

```bash=
bash test.sh
#test.sh 可改為自己或是其他人寫好的 .sh 檔
```

## Package file extension (deb, rpm)
  - **deb(Debian Package)**
    DEB 是由基於 Debian 的 Linux 發行版使用的封裝格式，包括 Debian 本身以及派生版如 Ubuntu 和 Linux Mint。
    可以使用 <b>dpkg</b> 套件安裝管理器進行套件的安裝、刪除與查詢。

    <b>How to run .deb file</b>

    ```bash=
    dpkg -i ${PACKAGE_FILE.deb}
    #${PACKAGE_FILE.deb} 可改為其他你打算安裝的 .deb 檔
    ```

  - **rpm(Red Hat Package Manager)**
    RPM 是由基於 Red Hat 的 Linux 發行版使用的封裝格式，包括 Red Hat Enterprise Linux（RHEL）、CentOS、Fedora 等等。
    可以使用 <b>rpm</b> 套件安裝管理器進行套件的安裝、刪除與查詢。

    ```bash=
    rpm -i ${PACKAGE_FILE.rpm} 
    #${PACKAGE_FILE.rpm} 可改為其他你打算安裝的 .deb 檔
    ```

## Archive file (壓縮檔)
壓縮檔檔案類型有幾種，這裡只會提供幾種比較常見的壓縮檔其壓縮與解壓縮方式，若有遇到沒在這篇教學看到的壓縮擋類型，可從 Reference 提供的網址或是自行上網查詢。

- **tar**

    打包

    ```bash=
    tar cvf ${FILE_NAME}.tar ${FILE_NAME}
    ```

    解包

    ```bash=
    tar xvf ${FILE_NAME}.tar 
    ```

- **gz**
    
    壓縮

    ```bash=
    gzip ${FILE_NAME}
    ```

    解壓縮

    ```bash=
    gunzip ${FILE_NAME}.gz
    ```
    ```bash=
    gzip -d ${FILE_NAME}.gz
    ```

- **tar.gz**
  
    壓縮

    ```bash=
    tar zcvf ${FILE_NAME}.tar.gz ${FILE_NAME}
    ```

    解壓縮

    ```bash=
    tar zxvf ${FILE_NAME}.tar.gz
    ```

- **.zip**

    壓縮

    ```bash=
    zip -r ${FILE_NAME}.zip ${FILE_NAME}
    ```

    解壓縮

    ```bash=
    unzip ${FILE_NAME}.zip
    ```


## Reference
1. [鳥哥-第十二章、學習 Shell Scripts](https://linux.vbird.org/linux_basic/centos7/0340bashshell-scripts.php)
2. [[Day 18] 自己的 Shell Script 自己寫 - 介紹篇](https://ithelp.ithome.com.tw/articles/10224799)
3. [RPM 套件安裝](https://dywang.csie.cyut.edu.tw/dywang/rhcsaNote/node82.html)
4. [GNU / Linux 各種壓縮與解壓縮指令
](http://note.drx.tw/2008/04/command.html)