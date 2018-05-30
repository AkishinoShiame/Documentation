## Abstract
# 概述

本文件為本人於2015年至2017年於研究所學習機器學習領域中的深度學習等相關知識領域的整理。盡可能的列舉出所學過的內容、包含理論的學習與理解等等，也同時將會把實作的相關成果做整理預紀錄。其中將也囊括了GPU運算之相關環境建置等等。並因應所需整理相關網站連結。
<br />

===

## 摘要

近年來台灣與諸多國家即將邁向高齡化社會，高齡化人口對於整體社會造成的影響將逐漸擴大。在高齡人口與生育率下降等因素的疊合下，台灣的撫養比也將失衡。而近期人工智慧在不同的專精領域下又佔得一席之地，如Google的Alpha Go與微軟於日本開發的AI「りんな」等皆已顯示出人工智慧的跟已逐漸扎穩。在種種的機緣與巧合下，為了減輕撫養負擔，銀法族長期照護機器人勢必成為一個明確的趨勢與方向。本研究之系統將利用聲頻圖進行深度卷積網路之訓練用以辨識年長者表達之情緒。並將此情緒結合使用者所表達之自然語言進行機器回話，建構出可應用於銀髮族之陪伴虛擬機器人之自然語言處理模型。本系統可全面性的偵測與分析出使用者講話時所表達的情緒並給予適度的正面回應，同時也提供正面的回話或建議等。由本研究提出之系統架構將分為兩個部分，使用者端藉由Unity開發出可同時編譯成Android或IOS的手機應用程式，而伺服器後端則利用Linux系統結合python語言建構網頁服務接口，使用GoogLeNet進行情緒辨識與seq2seq進行機器回話。本系統直接支援使用者以自然語言作為輸入，並做對應的處理後產生對應的動作作為情緒回覆以及回應對話。

## Abstract

This study presents a Virtual Elderly Companion Agent which based on speech spectrograms, seq2seq chatbot and deep convolutional neural networks. The system can auto-dynamically detect and analyze the user’s emotion from the dialogue and give appropriate positive emotion feedback. The proposed system architecture is divided into two parts. The client side uses Unity Editor to compose the mobile app, which supports both Android operating system and iPhone OS (iOS); the server side is implemented in python, and applied GoogLeNet for emotion recognition, and RNN-LSTM for Seq2Seq chatbot conversation. The system supports natural language as speech input, and then analyzes the converted speech spectrogram also the translated natural language text to provide appropriate feedback and conversations.