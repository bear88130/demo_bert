# demo_bert
 簡易BERT情緒分析


主要參考
[進擊的BERT](https://leemeng.tw/attack_on_bert_transfer_learning_in_nlp.html)  
從 BERT fine tune 下游任務 開始


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
