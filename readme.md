# 🎶 CompLex: Music Theory Lexicon Constructed by Autonomous Agents for Automatic Music Generation 

[![Dataset](https://img.shields.io/badge/Download-CompLex-green)](https://drive.google.com/drive/folders/1W9fW3m7zfsTzaUr3Rqi5t7hAa8R0dcMB?usp=sharing)  

---

## 📌 Overview  
**CompLex** is the first **automatically constructed music theory lexicon** designed to enhance text-to-music generation.  
Instead of relying solely on scarce and noisy music data, we let **LLMs educate LMMs** by injecting structured knowledge of music theory.  

Our contributions:  
- **CompLex**: A large-scale music theory lexicon with **37,432 items** across 9 categories and 90 properties.  
- **LexConstructor**: A novel multi-agent algorithm with **role-playing + QA strategy** to construct expert-level lexicons from just 9 keywords and 5 prompt templates.  
- **Applications**: Integrating CompLex into text-to-music models significantly improves **mood accuracy, genre accuracy, relevance, and overall music quality**.  

---

## 📂 Download CompLex  
The complete lexicon is provided as a single JSON file:  

👉 [**Download `complex.json` (Google Drive)**](https://drive.google.com/drive/folders/1W9fW3m7zfsTzaUr3Rqi5t7hAa8R0dcMB?usp=sharing)  

This file contains all categories, items, properties, and property–value pairs in a structured format.  


---

## 🚀 Quick Start  

```python
import json

# Load CompLex
with open("complex.json", "r") as f:
    complex_lexicon = json.load(f)

# Example: access a category
print(complex_lexicon["chord"][:2])  # prints first two chord entries
