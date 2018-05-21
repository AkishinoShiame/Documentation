# System
# 系統環境

### Content
## 目錄

* [前置作業](#Pre-Process)
* [Ubuntu Server 16.04 LTS](#ubuntu-server-1604)
* [Ubuntu Server 14.04 LTS](#ubuntu-server-1404)

### Pre-Process
## 前置作業

安裝Ubuntu系統將需要下載對應的iso進行安裝，因此需連線至[ubuntu-tw官方網站](https://www.ubuntu-tw.org/modules/tinyd0/)下載對應的版本與系統。

![img 1](img/Pic01.PNG) <br />

接著，將載下來的ISO以兩種方式皆可產生安裝媒體。

``` 方法1: ``` 
將ISO直接燒錄成光碟。

``` 方法2: ``` 
使用[Rufus軟體](https://rufus.akeo.ie/)建置安裝媒體，下載方式如下圖所示。 

![img 2](img/Pic02.PNG) <br />

## Ubuntu 14.04 Server

* UEFI BIOS bootup (較新的主機板)

![img 3](img/Pic03.PNG) <br />

* Legacy BIOS bootup (傳統開機方式)

![img 4](img/Pic04.PNG) <br />

![img 5](img/Pic05.PNG) <br />

接著安裝系統

選擇語言

![img 6](img/Pic06.PNG) <br />

選擇地區

![img 7](img/Pic07.PNG) <br />

選擇系統編碼

![img 8](img/Pic08.PNG) <br />

選擇鍵盤配置

![img 9](img/Pic09.PNG) <br />

![img 10](img/Pic10.PNG) <br />

等待系統自動設定

![img 11](img/Pic11.PNG) <br />

![img 12](img/Pic12.PNG) <br />

![img 13](img/Pic13.PNG) <br />

設定主機名稱

![img 14](img/Pic14.PNG) <br />

建立使用者帳戶

![img 15](img/Pic15.PNG) <br />

![img 16](img/Pic16.PNG) <br />

![img 17](img/Pic17.PNG) <br />

![img 18](img/Pic18.PNG) <br />

決定是否將個人資料夾進行加密

![img 19](img/Pic19.PNG) <br />

確認系統時區/時間

![img 20](img/Pic20.PNG) <br />

![img 21](img/Pic21.PNG) <br />

系統自動偵測硬碟/硬體配置

![img 22](img/Pic22.PNG) <br />

建立硬碟分割 (LVM為logical volume manager，多數伺服器建置時為後期硬體擴充方便而選擇此選項)

(本次安裝只使用簡易的方式分割)

![img 23](img/Pic23.PNG) <br />

選對要安裝的目標硬碟

![img 24](img/Pic24.PNG) <br />

注:通常Linux會有SWAP分割區，建議大小為記憶體的1.5~2倍。

* UEFI BIOS bootup (較新的主機板)
* 此方法會自動採用GPT磁碟切割表並進行分割，主要明顯差異是比傳統多EFI開機區

![img 25](img/Pic25.PNG) <br />

* Legacy BIOS bootup (傳統開機方式)
* 此方法會自動採用MBR磁碟切割表並進行分割

![img 26](img/Pic26.PNG) <br />

系統開始自動安裝

![img 27](img/Pic27.PNG) <br />

![img 28](img/Pic28.PNG) <br />

接著，詢問是否要使用proxy進行系統更新(空白為不使用)

![img 29](img/Pic29.PNG) <br />

系統更新中

![img 30](img/Pic30.PNG) <br />

![img 31](img/Pic31.PNG) <br />

決定系統是否往後自動更新

![img 32](img/Pic32.PNG) <br />

決定需額外安裝的伺服器程式

![img 33](img/Pic33.PNG) <br />

![img 34](img/Pic34.PNG) <br />

安裝完成，系統將重啟

![img 35](img/Pic35.PNG) <br />

![img 36](img/Pic36.PNG) <br />

![img 37](img/Pic37.PNG) <br />

## Ubuntu 16.04 Server

* UEFI BIOS bootup (較新的主機板)

* Legacy BIOS bootup (傳統開機方式)
