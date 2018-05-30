## Abstract
# 概述

本文件為本人於2015年至2017年於研究所學習機器學習領域中的深度學習等相關知識領域的整理。盡可能的列舉出所學過的內容、包含理論的學習與理解等等，也同時將會把實作的相關成果做整理預紀錄。其中將也囊括了GPU運算之相關環境建置等等。並因應所需整理相關網站連結。
<br />

---

---

## 摘要

近年來台灣與諸多國家即將邁向高齡化社會，高齡化人口對於整體社會造成的影響將逐漸擴大。在高齡人口與生育率下降等因素的疊合下，台灣的撫養比也將失衡。而近期人工智慧在不同的專精領域下又佔得一席之地，如Google的Alpha Go與微軟於日本開發的AI「りんな」等皆已顯示出人工智慧的跟已逐漸扎穩。在種種的機緣與巧合下，為了減輕撫養負擔，銀法族長期照護機器人勢必成為一個明確的趨勢與方向。本研究之系統將利用聲頻圖進行深度卷積網路之訓練用以辨識年長者表達之情緒。並將此情緒結合使用者所表達之自然語言進行機器回話，建構出可應用於銀髮族之陪伴虛擬機器人之自然語言處理模型。本系統可全面性的偵測與分析出使用者講話時所表達的情緒並給予適度的正面回應，同時也提供正面的回話或建議等。由本研究提出之系統架構將分為兩個部分，使用者端藉由Unity開發出可同時編譯成Android或IOS的手機應用程式，而伺服器後端則利用Linux系統結合python語言建構網頁服務接口，使用GoogLeNet進行情緒辨識與seq2seq進行機器回話。本系統直接支援使用者以自然語言作為輸入，並做對應的處理後產生對應的動作作為情緒回覆以及回應對話。

## Abstract

This study presents a Virtual Elderly Companion Agent which based on speech spectrograms, seq2seq chatbot and deep convolutional neural networks. The system can auto-dynamically detect and analyze the user’s emotion from the dialogue and give appropriate positive emotion feedback. The proposed system architecture is divided into two parts. The client side uses Unity Editor to compose the mobile app, which supports both Android operating system and iPhone OS (iOS); the server side is implemented in python, and applied GoogLeNet for emotion recognition, and RNN-LSTM for Seq2Seq chatbot conversation. The system supports natural language as speech input, and then analyzes the converted speech spectrogram also the translated natural language text to provide appropriate feedback and conversations.



|                                           論文資訊                                            |
|:---------------------------------------------------------------------------------------------:|
| ---------------:|:--------------------------------------------------------------------------- |
| 本論文永久網址:  | http://hdl.handle.net/11296/s73rsn |
| 研究生:    | [邱盛宇](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=auc=%22%E9%82%B1%E7%9B%9B%E5%AE%87%22.&searchmode=basic) |
| 研究生(外文):   | [CHIU, SHENG-YU](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=aue=%22CHIU%2C%20SHENG-YU%22.&searchmode=basic) |
| 論文名稱:    | 以深度網路建構自然語言處理模型 |
| 論文名稱(外文):  | Study on Natural Language Processing using Deep Neural Network |
| 指導教授:    | [李明哲](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=adc=%22%E6%9D%8E%E6%98%8E%E5%93%B2%22.&searchmode=basic) |
| 指導教授(外文):  | [LEE, MING-CHE](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=ade=%22LEE%2C%20MING-CHE%22.&searchmode=basic) |
| 口試委員:    | [蔡昆樺](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=sayc=%22%E8%94%A1%E6%98%86%E6%A8%BA%22.&searchmode=basic)、[謝東成](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=sayc=%22%E8%AC%9D%E6%9D%B1%E6%88%90%22.&searchmode=basic) |
| 口試委員(外文):  | [TSAI, KUN-HUA](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=saye=%22TSAI%2C%20KUN-HUA%22.&searchmode=basic)、[HSIEH, TUNG-CHENG](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=saye=%22HSIEH%2C%20TUNG-CHENG%22.&searchmode=basic) |
| 口試日期:    | 2017-07-03 |
| 學位類別:    | 碩士 |
| 校院名稱:    | [銘傳大學](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=sc=%22%E9%8A%98%E5%82%B3%E5%A4%A7%E5%AD%B8%22.&searchmode=basic) |
| 系所名稱:    | [資訊傳播工程學系碩士班](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=dp=%22%E8%B3%87%E8%A8%8A%E5%82%B3%E6%92%AD%E5%B7%A5%E7%A8%8B%E5%AD%B8%E7%B3%BB%E7%A2%A9%E5%A3%AB%E7%8F%AD%22.&searchmode=basic) |
| 學門:     | 傳播學門 |
| 學類:     | 一般大眾傳播學類 |
| 論文出版年:   | 2017 |
| 畢業學年度:   | 105 |
| 語文別:    | 中文 |
| 論文頁數:    | 109 |
| 中文關鍵詞:   | [老人照護](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=kwc=%22%E8%80%81%E4%BA%BA%E7%85%A7%E8%AD%B7%22.&searchmode=basic)、[深度學習](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=kwc=%22%E6%B7%B1%E5%BA%A6%E5%AD%B8%E7%BF%92%22.&searchmode=basic)、[深度卷積網路](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=kwc=%22%E6%B7%B1%E5%BA%A6%E5%8D%B7%E7%A9%8D%E7%B6%B2%E8%B7%AF%22.&searchmode=basic)、[GoogLeNet](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=kwc=%22GoogLeNet%22.&searchmode=basic)、[機器應答](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=kwc=%22%E6%A9%9F%E5%99%A8%E6%87%89%E7%AD%94%22.&searchmode=basic) |
| 外文關鍵詞:   | [Elderly Companion](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=kwe=%22Elderly%20Companion%22.&searchmode=basic)、[Deep Convolutional Neural Network](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=kwe=%22Deep%20Convolutional%20Neural%20Network%22.&searchmode=basic)、[AlexNet](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=kwe=%22AlexNet%22.&searchmode=basic)、[GoogLeNet](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=kwe=%22GoogLeNet%22.&searchmode=basic)、[RNN-LSTM](https://ndltd.ncl.edu.tw/cgi-bin/gs32/gsweb.cgi/ccd=xAGuAl/search?q=kwe=%22RNN-LSTM%22.&searchmode=basic) |