# Event Causality Identification via Structure optimization and Reinforcement Learning


## GenSORL

# Requirements

The dependency packages can be installed with the command:

```
pip install -r requirements.txt
```


Datasets
==========
1. 下载数据集 (建议略过该步, 直接进行[2]和Step 3)  
    [EventStoryLine](https://github.com/tommasoc80/EventStoryLine)  
    [Causal-TimeBank](https://github.com/paramitamirza/Causal-TimeBank)
2. 下载论文作者使用的数据
    [全部数据(Google Drive)](https://drive.google.com/drive/folders/1juvVPa7wqYqBYzj-wvpwbBKV3Jkufk11?usp=sharing)  
3. 解压覆盖  
    步骤[1]-->解压文件夹, 将数据集复制到`datasets`文件夹下  
    步骤[2]-->解压文件夹至项目文件夹下，覆盖原来的`datasets`文件夹
# Usage

1. Prepare data\
Extract data from the ESL dataset: In the preprocessor.py file located at ```.\datasets\preprocessor.py```, set ```dataset = 'ESL'```.<br>
Extract data from the Causal-TB dataset: In the preprocessor.py file located at ```.\datasets\preprocessor.py```, set ```dataset = 'Causal-TB'```.<br>
and run:

```
python datasets/preprocessor/preprocessor.py
```


2. Train model:
```
sh ESL_bash.sh
```
or Select training dataset: In the datasets.py file located at ```.\data_modules\datasets.py```, change "ESL" to "Causal-TB" in line 143.
```
sh CausalTB_bash.sh
```


# Acknowledgement
Part of our code is borrowed from [code](https://github.com/hieumdt/GenECI), many thanks.
