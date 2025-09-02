# Wikipedia-NLP-Practice: Bigram Analysis with PySpark  

## Project Objective  
This project applies PySpark to perform Natural Language Processing (NLP) on a Wikipedia dataset, focusing on sentence structure and bigram frequency analysis. The results are compared with the **MAGPIE idiom dataset** to investigate the relationship between frequent word pairs and idiomatic expressions.  

---

## Workflow  

1. **Data Loading**  
   - Load the Wikipedia dataset (CSV format).  
   - Load the MAGPIE idiom dataset (JSONL format).  

2. **Exploratory Analysis**  
   - Count the **number of unique sentences**: 389,639.  
   - Calculate **word count per sentence** and derive bigram counts.  
   - Compute **average bigram count**: 18.04.  

3. **Bigram Frequency Analysis**  
   - Extract the top 10 most frequent bigrams from Wikipedia:  
     - "of the" (76,294)  
     - "in the" (54,058)  
     - "to the" (25,486)  
     - "at the" (21,596)  
     - …  

4. **Cross-check with MAGPIE Idioms**  
   - Identified **67 bigrams** overlapping with MAGPIE idioms.  
   - After excluding idioms, extracted **ranked bigrams from 2500–2510**, e.g.:  
     - 2500: "to complete" – 176  
     - 2501: "was responsible" – 176  
     - 2509: "first team" – 175  

---

## Findings  
- Frequent bigrams in Wikipedia are dominated by function word combinations (e.g., "of the", "in the").  
- A small subset overlaps with the idiom dataset, highlighting linguistic connections between collocations and idiomatic expressions.  
- Mid-ranked bigrams (e.g., "to complete", "was responsible") carry more semantic information, useful for downstream NLP tasks.  

---

## How to Run  

1. **Clone the repository**  
   ```bash
   git clone https://github.com/your-username/Wikipedia-NLP-Practice.git
   cd Wikipedia-NLP-Practice
