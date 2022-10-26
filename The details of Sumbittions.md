# The details of Sumbittions

## PreProcess.ipyng
Here we Preprocess the raw data, concatenate the prompt, and utterance with same conv_id.
In other ipynb files, we will use the same preprocessed data.


## NewData Folder
We put the new data here including new_train.csv, valid.csv, and test.csv.


## TPU_Roberta_Best_Score.ipynb
This code run on TPU and had the best result on Kaggle
![](https://i.imgur.com/1YLjHHy.png)


The pretrained model we use is:
```
model_name = "Nakul24/RoBERTa-emotion-classification"
``` 

To improve the performance and robustness, we resample the training data, and each label would have 2000 numbers of data.

After finding the best hyperparameter for the result:
```
lr = 1e-5
epcho = 1
```
![](https://i.imgur.com/ezoCR3o.png)

We add the valid_data in train_data to train the model.


