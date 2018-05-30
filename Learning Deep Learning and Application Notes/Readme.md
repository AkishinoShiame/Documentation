# Learning Deep Learning and Application Notes


> 本文件整理碩士論文研究期間所獲得的相關理論與實驗後的經驗與資訊。期間包含深度學習相關理論知識，與建立於深度學習之上的圖像訓練和文字訓練。
> 
> 相關已完成的應用請參照[此Repo](https://github.com/artmusic0/Graduated-Project)

### Abstract
## 概述

[傳送門](Ch0-Abstract)

### Content
## 目錄

* [概述](#abstract)
* [系統環境](#system)
    * [前置作業](#前置作業)
	* [Ubuntu Server 14.04 LTS](#ubuntu-1404-server)
	* [Ubuntu Server 16.04 LTS](#ubuntu-1604-server)
	* [網路設置(Optional)](#網路設置optional)
* [Python基礎與IDE](#python-basics)
    * [Python與版本](#python與版本)
    * [Python函式庫](#python函式庫)
    * [Python語言](#python語言)
    * [Python編輯器](#python編輯器)
* [GPU運算建置-CUDA](#gpu-cuda)
    * [Windows環境](#Windows環境)
    * [Linux環境](#Linux環境)
* [深度網路理論整理](#deep-learning)
    * [分類問題](#分類問題)
      * [線性回歸](#線性回歸)
      * [非線性回歸](#非線性回歸)
      * [SVM](#SVM)
    * [類神經網路](#類神經網路)
      * [非線性化方法](#非線性化方法)
      * [選擇性錯誤評估函式](#選擇性錯誤評估函式)
      * [全連結神經網路](#全連結神經網路)
    * [卷積神經網路](#卷積神經網路)
    * [遞歸神經網路](#遞歸神經網路)
      * [LSTM法](#LSTM法)
      * [應用範圍](#應用範圍)
    * [自然語言處理](#自然語言處理)
      * [情緒認知](#情緒認知)
      * [文字(詞)向量](#文字詞向量)
        * [One-Hot Vector](#one-hot-vector)
    	* [Word2Vec](#word2vec)
      * [Seq2Seq](#seq2seq)
    * [微軟日本(りんな)ChatBot研究](#微軟日本りんなchatbot研究)
      * [翻訳モデル](#翻訳モデル)
      * [文の長さ](#文の長さ)
      * [AIM言語モデル](#aim言語モデル)
      * [GRU類似度](#gru類似度)
* [API應用程式界面](#api)
    * [Theano](#theano)
    * [TensorFlow](#tensor-flow)
    * [DIGITS](#digits)
    * [Keras](#keras)
    * [Caffe](#caffe)
    * [Torch](#torch)
	* [Others](#others)
* [注意事項](#caution)

<br />

### System
## 系統環境

[傳送門](Ch1-System)

> ### 前置作業
> 
> [傳送門](Ch1-System#pre-process)
> 
> ### Ubuntu 14.04 Server
> 
> [傳送門](Ch1-System#ubuntu-1404-server)
> 
> ### Ubuntu 16.04 Server
> 
> [傳送門](Ch1-System#ubuntu-1604-server)
> 
> ### 網路設置(Optional)
> 
> [傳送門](Ch1-System#internet-settings)
  
### Python Basics
## Python基礎與IDE

[傳送門](Ch2-Python-Basics)

> ### python與版本
> 
> [傳送門](Ch2-Python-Basics#python與版本)
> 
> ### python函式庫
> 
> [傳送門](Ch2-Python-Basics#python函式庫)
> 
> ### python語言
> 
> [傳送門](Ch2-Python-Basics#python語言)
> 
> ### python編輯器
> 
> [傳送門](Ch2-Python-Basics#python編輯器)

### GPU CUDA
## GPU運算建置-CUDA

[傳送門](Ch3-GPU-Cuda)

> ### Windows環境
> 
> [傳送門](Ch3-GPU-Cuda#windows-cuda)
> 
> ### Linux環境
> 
> [傳送門](Ch3-GPU-Cuda#linux-cuda)

### Deep Learning
## 深度網路理論整理

[傳送門](Ch4-Deep-Learning)

> ### 分類問題
> 
> [傳送門](#)
> 
> > ###  線性回歸
> >  
> >  [傳送門](#)
> >  
> > ###  非線性回歸
> >  
> >  [傳送門](#)
> >  
> > ###  SVM
> >  
> >  [傳送門](#)
>   
> ###  類神經網路
> 
> [傳送門](#)
> 
> > ###  非線性化方法
> >  
> >  [傳送門](#)
> >  
> > ### 選擇性錯誤評估函式
> >  
> >  [傳送門](#)
> >  
> > ### 全連結神經網路
> >  
> >  [傳送門](#)
>   
> ### 卷積神經網路
> 
> [傳送門](#)
> 
> ### 遞歸神經網路
> 
> [傳送門](#)
> 
> > ###  LSTM法
> >  
> >  [傳送門](#)
> >  
> > ###  應用範圍
> >  
> >  [傳送門](#)
>   
> ###  自然語言處理
> 
> [傳送門](#)
> 
> > ###  情緒認知
> >  
> >  [傳送門](#)
> >  
> > ###  文字(詞)向量
> >  
> >  [傳送門](#)
> >  
> > > ###  One-Hot Vector
> > > 
> > > [傳送門](#)
> > > 
> > > ###  Word2Vec
> > > 
> > > [傳送門](#)
> >	
> > ###  Seq2Seq
> > 
> > [傳送門](#)
>   
> ###  微軟日本(りんな)ChatBot研究
> 
> [傳送門](#)
> 
> > ###  翻訳モデル
> >  
> >  [傳送門](#)
> >  
> > ###  文の長さ
> >  
> >  [傳送門](#)
> >  
> > ###  AIM言語モデル
> >  
> >  [傳送門](#)
> >  
> > ###  GRU 類似度
> >  
> >  [傳送門](#)
  

### API
## 應用程式界面

[傳送門](Ch5-API)

> ### Theano
> 
> [傳送門](#)
> 
> ### Tensor Flow
> 
> [傳送門](#)
> 
> ### DIGITS
> 
> [傳送門](#)
> 
> ### Caffe
> 
> [傳送門](#)
> 
> ### Torch
> 
> [傳送門](#)
> 
> ### Others
> 
> [傳送門](#)

### Caution
## 注意事項

硬體對應考量與訓練中的部分細節須注意之處。
