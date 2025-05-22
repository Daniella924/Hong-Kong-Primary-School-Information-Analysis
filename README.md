# 🏫 Hong Kong Primary School Information Analysis 

## 📌 Project Overview  

This project focuses on processing and analyzing primary school information data in Hong Kong. The system includes data cleaning pipelines, missing value handling strategies, and automated data quality verification.  

## ✨ Key Features  

### 1. 🧹 Traditional Chinese Cleaning Pipeline  
- Developed an efficient text cleaning system specifically for Traditional Chinese content  
- Utilizes **regular expressions** to filter special symbols and non-standard characters  
- Achieves **processing speed of 5,000 records per minute** ⚡  

### 2. 🔍 Hybrid Missing Value Processing  
- Implemented a **dual-strategy approach** for handling missing values:  
  - **🔢 Numeric fields**: KNN imputation with `k=5` neighbors  
  - **📝 Categorical fields**: Mode imputation + missing value markers 🏷️  
- Ensures proper handling of different data types while preserving missingness info  

### 3. ✅ Automated Data Quality Verification  
- Built **robust validation** using **Great Expectations** library 🛡️  
- Defined **42 data quality constraints**, including:  
  - Teacher education field **must contain "Bachelor" / "Master" / "PhD"** 🎓  
  - Other domain-specific rules to ensure **data integrity** ✔️  

## 📂 Repository Structure  

```
├── 📁 data_cleaning/          # 🧼 Traditional Chinese text cleaning pipeline  
├── 📁 missing_value_handling/ # 🔄 Hybrid missing value processing  
├── 📁 data_validation/        # ✅ Automated quality verification  
├── 📁 docs/                   # 📝 Documentation & notes  
├── 📁 tests/                  # 🧪 Unit & integration tests  
└── 📄 README.md               # This file  
```  

## ⚙️ Requirements  

- **Python 3.8+** 🐍  
- Required packages:  
  - `pandas` 🐼  
  - `scikit-learn` (for KNN imputation)  
  - `great-expectations` 🎯  
  - `regex` (for advanced regex)  

## 🚀 Usage  

1. Clone the repo: `git clone [repo-url]`  
2. Install dependencies: `pip install -r requirements.txt`  
3. Run cleaning pipeline: `python data_cleaning/main.py`  
4. Handle missing values: `python missing_value_handling/processor.py`  
5. Validate data: `python data_validation/validate.py`  

## 🤝 Contribution  

Contributions are welcome! 🎉  
- 🐛 Found a bug? **Open an issue!**  
- 💡 Have an improvement? **Submit a PR!**  

Let's make this project even better! 🚀
