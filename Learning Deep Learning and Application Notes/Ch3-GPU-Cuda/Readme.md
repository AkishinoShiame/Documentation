# GPU-CUDA
# GPU運算建置-CUDA

本章節就windows 10與Linux ubuntu 14.04/16.04安裝 CUDA的步驟與細節進行探討與整理。 此處須注意的是由於不同系統設計架構的關係，於windows上安裝時須同時事先安裝對應版本的Visual Studio以便系統進行編譯與執行。Linux上需注意的是對應的驅動版本與在Cuda安裝時產出對應的安裝選項。
底下將分兩個區塊進行講解。
同時，無論是在哪個平台安裝Cuda，須注意要額外再下載與安裝CuDnn，此為運行深度學習相關程式的必須套件，用以加速硬體運算效能。

### Content
## 目錄

* [Windows環境](#Windows-cuda)
* [Linux環境](#linux-cuda)

### Windows Cuda

於windows上安裝Cuda前，需根據對應的顯卡硬體，事先檢查所持有的卡片是否支援。由<a src=” https://developer.nvidia.com/cuda-gpus”>此處</a>或是利用型號尋找官方頁面得知是否支援。

接著，由官方的<a src=” http://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html”>系統需求</a>頁面對應使用的系統版本與確定對應需安裝的Visual Studio版本。

-----------------------------------------------------
-----------------------------------------------------
表格節錄，收錄時間 JST 30/03/16 請在安裝前注意ChangeLog
-----------------------------------------------------

| Operating System       | Native x86_64 | Cross (x86_32 on x86_64)|
|:---------------------- |:-------------:|:-----------------------:|
| Windows 10             |    YES        |      YES                |
| Windows 8.1            |    YES        |      YES                |
| Windows 7              |    YES        |      YES                |
| Windows Server 2016    |    YES        |      NO                 |
| Windows Server 2012 R2 |    YES        |      NO                 |

| Compiler                   | IDE                          | Native x86_64 | Cross (x86_32 on x86_64) |
|:-------------------------- |:---------------------------- |:-------------:|:------------------------:|
| Visual C++ 15.0            | Visual Studio 2017           | YES           | NO                       |
| Visual C++ 14.0            | Visual Studio 2015           | YES           | NO                       |
|   --                       | Visual Studio Community 2015 | YES           | NO                       |
| Visual C++ 12.0            | Visual Studio 2013           | YES           | YES                      |
| Visual C++ 11.0            | Visual Studio 2012           | YES           | YES                      |
| Visual C++ 10.0 DEPRECATED | Visual Studio 2010           | YES           | YES                      |

-----------------------------------------------------
-----------------------------------------------------

### Linux Cuda


