# Docker basics


**This document will wrote about the basics of docker container.<br>
本文件將簡述Docker 與 docker container的相關資訊與簡單的使用方式。**


## Content
* [Docker概念](#Docker概念)
* [Docker安裝](#Docker安裝)
* [Docker使用](#Docker使用)


#### Docker概念
### Docker concept

====================

Docker 原概念為為了節省系統的龐大性並節省不必要且重複的底層環境而產生出的概念與架構。 基本上皆針對Linux系統所進行開發。

而Container的原始概念就是將環境包裝成一個封閉式環境，就像是貨櫃箱一樣。 將所有的環境與系統變數等鎖定在同一個Container裡。

之後，有人就想到了將兩個概念與做法進行結合，產生出Docker container的架構，並在部分需求的狀況下，提供少部分的開放性給Container。 可將外部的儲存空間掛載(mount)至docker container內提供使用。

其整體架構為，將底層系統與部分共同性的部分直接成為HOST，而docker container的image只包裝非前述但所需之環境變數，程式與執行資訊等資料進行包裝，並直接以執行緒(Thrad)的角度來運作整個服務。

該[官網](https://www.docker.com/)如下圖所示。

![img 1](img/Pic01.PNG) <br />

同時，建議初次使用的人可申請一個免費的[Docker Hub](https://hub.docker.com/)帳號，方便往後可下載相關的image或是相關開發上的使用。

![img 2](img/Pic02.PNG) <br />

由於Docker目前已Linux的架構為主，因此若將Docker執行在windows系統上或是MAC OS上，其會使用[Vbox](https://www.virtualbox.org/)並結合kubernetes程式來管理並建置一個虛擬的Linux環境供docker使用。

此外，Docker本身有額外為windows版提供新的架構，除了使用Vbox外，此新版的結合了Windows內含的Hyper-V以執行更穩定的架構。

#### Docker安裝
### Docker Install



#### Docker使用
### Docker Usage


