# 訓練 BERT 情緒正負向模型

### 說明
主要用於理解模型建立，並不是用於專業場域

主程式為 train_title.ipynb，裡面有 訓練model 和 預測  
個人測試可以建立模型和預測    
準確度很高，但訓練資料量不多，`不能真的拿來實用`

### 主要參考
[進擊的BERT](https://leemeng.tw/attack_on_bert_transfer_learning_in_nlp.html)  
從 BERT fine tune 下游任務 開始

### python環境建立
pytorch 需要根據環境產生指令去安裝 [pytorch環境產生指令](https://pytorch.org/get-started/locally/)  
需要替換的指令為下行  
conda install pytorch torchvision torchaudio pytorch-cuda=11.6 -c pytorch -c nvidia  

安裝指令  
```cmd
conda update -n base -c defaults conda
conda create -n demo_bert python=3.10

conda activate demo_bert
pip install pandas numpy transformers tqdm requests chardet jieba scikit-learn regex tensorflow

conda install pytorch torchvision torchaudio pytorch-cuda=11.6 -c pytorch -c nvidia

pip install ipykernel
python -m ipykernel install --user --name=demo_bert
conda deactivate
```

