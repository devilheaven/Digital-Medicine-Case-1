|-code
|--version2.ipynb 
|--version3.ipynb
|-output_vsersion2.csv
|-output_vsersion3.csv

----

# 關鍵字詞
* [國家教育研究院](https://terms.naer.edu.tw/download/)
  * 內分泌學名詞
  * 病理學名詞
* Recognizing Obesity and Comorbidities in Sparse Data 表格一
* 其他可能與肥胖相關醫學關鍵字詞

# version2
## 資料前處理
* 將電子病歷中的符號替換成空格
* 將電子病歷文本及關鍵字詞以空格進行切割
## 特徵擷取
* 計算文本中單一字詞出現次數，並找群其中醫學相關字詞出現次數

## 機器學習
使用scikit-learn的random forest建立模型
參數:n_estimators=100000,max_depth=10

## 輸出
validation dataset的預測結果，儲存至output_version2.csv

# version3
## 資料前處理
* 將電子病歷中的符號替換成空格

## 特徵擷取
* 計算文本中醫學相關字詞組合出現次數

## 機器學習
使用scikit-learn的random forest建立模型
參數:n_estimators=100000,max_depth=10

## 輸出
validation dataset的預測結果，儲存至output_version3.csv