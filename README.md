# **專案說明**

## **來源**
[whisper_streaming_CN](https://github.com/Gloridust/whisper_streaming_CN)

---

## **環境需求**

### **基本環境**
- **Python 版本**：`Python = 9.2.0`
- **CUDA 版本**：`CUDA 12.1.0`
- **cuDNN 版本**：`cuDNN 9.1.0`

### **所需套件**
- `faster-whisper`
- `sounddevice`
- `numpy`
- `librosa`
- `opencc`

---

## **目錄結構與檔案說明**

### **1. Real_Time 資料夾**
包含所有與即時轉錄相關的檔案。

#### **1.1 microphone.py**
- **用途**：  
  使用麥克風進行即時聲音轉文字。

#### **1.2 simulate_realtime.py**
- **用途**：  
  模擬實時音檔處理，適用於當下無法使用麥克風的情況。

#### **1.3 example.mp3**
- **用途**：  
  測試音檔（中文音頻）。

---

### **2. Non_Real_Time 資料夾**
包含所有與非即時轉錄相關的檔案。

#### **2.1 translation.py**
- **用途**：  
  將 `translation_file/input` 資料夾中的 MP3 音檔轉錄為字幕檔，並輸出至 `translation_file/output` 資料夾。

#### **2.2 translation_file 資料夾**
存放用於非即時轉錄的輸入與輸出文件。

- **Input 資料夾**：  
  存放待處理的音檔（MP3 格式）。

- **Output 資料夾**：  
  存放轉錄完成的字幕檔案（TXT 格式）。

---
