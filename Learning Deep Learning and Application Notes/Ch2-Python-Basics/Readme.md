# Python Basics
# Python基礎與IDE

### Content
* [Python與版本](#python與版本)
* [Python函式庫](#python函式庫)
* [Python語言](#python語言)
* [Python編輯器](#python編輯器)

## Python與版本

Python 程式語言與其他以往的程式語言的邏輯上接近，但是程式的撰寫方式注重於排版。其編譯方式由排版的縮排架構進行解讀。

其中，包含幾個特點包含list架構，資料處理的便利性，與多元又開放的函式庫等等。

目前主流的是Python 3.4 與 3.5。　Python 2.7也是許多人在使用的，但因為有[相關資訊](https://www.python.org/dev/peps/pep-0373/)透露出2.7版要在近期內終止支援。

因此有人因此額外提供[相關網頁](https://pythonclock.org/)來Count Down Python 2的殘存時間。

現今，不論使用的是哪個版本，皆已有足夠的對應函式庫可供使用。

## Python函式庫

### メニュー
* 安裝與使用
  * Windows安裝方式
  * Linux(Ubuntu)安裝方式
  * Mac安裝方式
* 常用函式庫


* 安裝與使用
  * Windows安裝方式
  
  Python安裝方式建議直接從官方網站下載，並在安裝時注意相關的路徑與內建工具需勾選與安裝。
  
  根據系統不同請選擇對應的位元數進行安裝。 請參照Windows 設定中的系統做確認。
  
  ![img 01](img/Pic01.PNG)
  
  對應下載頁面，選擇合適的安裝檔下載。
  
  ![img 02](img/Pic02.PNG)
  
  確認安裝
  
  ![img 03](img/Pic03.PNG)
  
  如果要加裝外部的函示庫，則開啟cmd使用內建提供之pip工具進行安裝。
  
  ![img 04](img/Pic04.PNG)
  
  PS. 由於python本身會將不同版本分路徑安裝，因此若有開發需要可將多個不同版本的python安裝於同一電腦內。

* 安裝與使用
  * Linux(Ubuntu)安裝方式
  
  建議使用指令進行安裝，其相關完整安裝指令如下。
  
  ```bash
  
  #注意，根據不同的版本需求請將python換成"python2","python2.7","python3","python3.5"或"python3.6"等等
  
  sudo apt install python python-dev #python 主要套件
  sudo apt install python-pip #python 函式庫管理套件
  sudo apt install python-virtualenv #因應開發需求可額外安裝的套件
  
  ```
  
  ![img 05](img/Pic05.PNG)
  
  同時，在ubuntu中有主要兩種套件安裝方式:
    * 使用apt進行安裝
	* 使用pip進行安裝
  
  在我個人使用上比較建議使用pip進行安裝，由於此工具為python官方提供之套件，並且版本通常比較新也可選擇特定版本安裝。
  
  ```bash
  #apt安裝方法
  sudo apt install -y python-??? #將"python-???"改成想安裝的lib名稱，Ex:"python-numpy"
  
  ```
  
  ![img 06](img/Pic06.PNG)
  
  ```bash
  #pip安裝方法
  pip install ??? #將"???"改成要安裝的lib名稱，Ex:"numpy"
  
  ```
  
  ![img 07](img/Pic07.PNG)

* 安裝與使用
  * Mac安裝方式
  
  mac本身預設是會安裝python2，如下圖所示。
  
  ![img 08](img/Pic08.PNG)
  
  但此版本本身不含pip函式庫管理套件，因此需額外用指令進行安裝。
  
  ```bash
  
  sudo easy_install pip
  
  ```
  
  如此一來，即可直接使用pip指令進行套件安裝。
  
  ![img 09](img/Pic09.PNG)
  
  同時，在使用pip安裝套件時會得知需要加裝Xcode才有辦法完整運作，因此需下載免費的Xcode套件
  
  ![img 10](img/Pic10.PNG)
  
  如果要使用Python3，則常用的方式有兩種安裝方式：
	* Homebrew蘋果用套件管理程式
	* 官方GUI介面
  
  <br>
  
  **>Homebrew蘋果用套件管理程式<**
  
  根據Homebrew[官方](https://brew.sh/)網站所示，使用以下指令進行安裝Homebrew，接著可直接利用Homebrew快速安裝python3套件。
  
  ![img 11](img/Pic11.PNG)

  ```bash
  
  /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)" #安裝Homebrew
  
  brew update
  brew install python3 #更新與安裝python3
  
  ```
  ![img 12](img/Pic12.PNG)

  ![img 13](img/Pic13.PNG)

  ![img 14](img/Pic14.PNG)

  ![img 15](img/Pic15.PNG)

  **>官方GUI介面<**
  
  直接到官方下載mac專用安裝程式(.dmg)進行GUI安裝。

  ![img 16](img/Pic16.PNG)

  ![img 17](img/Pic17.PNG)

  ![img 18](img/Pic18.PNG)

  ![img 19](img/Pic19.PNG)

  安裝好後即可在終端機使用pip3安裝其他函式庫。

  ![img 20](img/Pic20.PNG)

* 常用函式庫

[NumPy](http://www.numpy.org/):

數值計算使用，在較為大的數值運算，矩陣運算與多為矩陣處理非常好用。

同時，此函式支援及時更新與儲存功能。

[SciPy](https://www.scipy.org/):

某種程度上來說可算是為前一函式庫(NumPy)的進階版。

其中專注於科學上的計算與使用，像是一些既定公式都可以在此找到。

[Pandas](https://pandas.pydata.org/):

接近於資料分析工具，其中拿來做資料的前處理時是個好用的工具。

[Matplotlib](https://matplotlib.org/):

Python中其中一種繪圖程式，在資料處理中常被拿來做資料視覺化的工具。

其內建強大的不同圖表工具幫助資料快速視覺化。

[NTLK](https://www.nltk.org/):

自然語言處理相關的常用函式庫，主要是用來做字詞的"tokenlize"。

可以把自然語言轉換為數值形式方便儲存與運算。

[Gensim](https://radimrehurek.com/gensim/):

略為接近前者，主要用來進行自然語言的文本分析，從文本內抽出並計算詞向量。

支援常見的兩種詞向量計算與通用格式。

此外，目前他本身也支援作文本向量與句子向量運算，為自然語言處理中一極為便利的工具。

[Scrapy](https://scrapy.org/):

python中知名的爬蟲工具，內建極為強大的爬蟲用分析工具。

可針對諸多需求進行變形，抓取所需要的資料。並可同時爬取非文本資料。

[Flask](http://flask.pocoo.org/):

使用python語言建置的網頁伺服器，類似apache, IIS等伺服器之功能。

可直接用python語言結合網頁語言(HTML, JavaScript, CSS...)等等混合使用做出簡易又華麗的網頁。

也適合來做產生API介面之工具。

[Pickle](https://docs.python.org/3/library/pickle.html)/[cPickle](https://docs.python.org/2.5/lib/module-cPickle.html):

Python內建的一個資料序列化儲存工具。

適合用來將把訓練好的權重等資訊進行壓縮與序列化儲存到電腦中。

有需要的時候也可直接叫出來使用，概念有點像是7-zip的資料封存。

PS.其他相關深度學習之lib將另外獨立章節說明。

## Python語言

以下簡單列舉Python程式語言的大致樣貌。

```python3 {.line-numbers}

# 以下為匯入函式庫的方式，此外python不限定只用系統安裝的，也可把寫好的py檔當成lib import
import os	#整包直接匯入，然後調用時直接使用os調用
import tensorflow as tf	#匯入後改名，使用時用tf調用
from numpy import random	#從整包的函式庫只匯入部分/單一function使用，調用時使用random調用
from keras.models import Sequential as kar_seq	#從整包的函式庫只匯入部分/單一function使用，調用時使用kar_seq調用

# 以下為變數宣告方式，python中的變數沒有預設宣告格式的功能。
values = [{"name": "Michelangelo", "food": "PIZZA"}, {"name": "Garfield", "food": "lasagna"}]
temp = 2
check = True


# def 開頭的為宣告function的功能，同時宣告後可直接被其他py檔案調用
def unpacker(name=None, food=None):
    return ["Hi, I'm {} and I love to eat {}!".format(name, food)]	#.format是一種python內建方便的功能，可以將對應的資訊往所要存放的位置塞入。

def string_factory(values):
    ans = []
    for value in values:	# for的其中一種方式，當value是陣列或是list時，python會自動抓取並一筆一筆丟入直到EoF。
        template = unpacker(**value)
        ans.extend(template)
    return ans

if __name__ == "__main__":
    result = string_factory(values) #調用def定義好的function，跟其他程式語言相同
    print(result)	#列印變數，將所要印的東西全都用()括起來，在python2只有"print result"的方式，無括弧。
	
	for i in range(10):	#for 抓取變數更新的另一種方式，從0開始到9，當到10會跳出迴圈。
		print(i)
		print(type(i), type(result))	#用type()內建函數可確認變數被給定的型態，並利用","可同時列印多個不同變數。

#別忘記python本身很重視排版，當縮排有錯將會導致執行錯誤。
```

## Python編輯器

list
* 集合包
  * WinPython
  * Anaconda
* 純編譯器
  * IDLE
  * Spyter
  * PyCharm
  * Others