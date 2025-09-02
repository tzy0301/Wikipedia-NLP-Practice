# Wikipedia-NLP-Practice: 使用 PySpark 的雙詞組分析  

## 專案目標  
本專案利用 PySpark 對 Wikipedia 語料進行自然語言處理 (NLP)，分析句子結構與雙詞組 (bigrams) 的出現頻率，並與 **MAGPIE idiom dataset** 進行比對，探討常見搭配詞與成語的關聯。  

---

## 工作內容  

1. **資料讀取**  
   - 載入 Wikipedia 語料（CSV 格式）。  
   - 載入 MAGPIE idiom dataset（JSONL 格式）。  

2. **探索性分析**  
   - 計算 **唯一句子數量**：389,639。  
   - 計算每句話的 **單詞數與雙詞組 (bigrams)**。  
   - 計算 **平均 bigram 數**：18.04。  

3. **Bigram 頻率分析**  
   - 找出 Wikipedia 最常見的前 10 bigrams：  
     - "of the" (76,294)  
     - "in the" (54,058)  
     - "to the" (25,486)  
     - "at the" (21,596)  
     - …  

4. **與 MAGPIE Idioms 比對**  
   - 發現 **67 個 Wikipedia bigrams** 出現在 MAGPIE idioms。  
   - 排除成語後，擷取 **排名 2500–2510 的 bigrams**，例如：  
     - 2500: "to complete" – 176  
     - 2501: "was responsible" – 176  
     - 2509: "first team" – 175  

---

## 專案成果  
- Wikipedia 語料中的常見 bigrams 多為功能詞組合（例如 "of the", "in the"）。  
- 少部分與 idioms 資料集重疊，顯示常用搭配與成語之間存在語言學連結。  
- 排名中段的 bigrams（如 "to complete", "was responsible"）更具語意資訊，可能適合進一步 NLP 任務。  

---

## 使用方法  

1. **Clone 專案**  
   ```bash
   git clone https://github.com/your-username/Wikipedia-NLP-Practice.git
   cd Wikipedia-NLP-Practice
2. **安裝並執行 Notebook**
   pip install pyspark\n
   開啟 INF6032_240217316.ipynb\n
   選擇 PySpark kernel，逐步執行各 cell。
