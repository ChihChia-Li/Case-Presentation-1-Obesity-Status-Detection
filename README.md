# Case-1_Obesity-Status-Detection
## Digital Medicine 2021 

### Task Overview
In this case, we are required to detect the obesity status of a patient via his/her electronic medical discharge record. It can be divide to two kinds of electronic records, including textual and intuitive. Textual kind record contains certain words, such as "obesity", "obese" that can help us easily classify the obesity status of the patient. On the other hand, intuitive kind record relies on the intuition of doctors to inference the obesity status via other relational informations contatined in the record. Our task is to train a classfier that can detect the obesity status either the record is textual kind or intuitive kind.

### Basic Requirements
* Python==3.7
* keras==2.6.0
* nltk==3.2.5
* pandas==1.1.5
* tqdm==4.62.3
* scikit-learn==0.22.2.post1
* tensorflow==2.6.0
* numpy==1.19.5
others are as colab environments

### Reproducing Submission
To reproduce my result, do the following steps:
1. Dataset Preparation
2. Train from scratch or Download Pretrained models
3. Inference

### Dataset Preparation
* Traning, Testing and validation text files need to be placed in different folders 
```
Case Presentation 1 Data
    +- Train_Textual
    |  U_ID_2.txt
    |  U_ID_4.txt
    |  ...
    |  ...
    +- Test_Intuitive
    | N_ID_55.txt
    | N_ID_59.txt
    | ...
    | ...
    +- Validation
    | ID_1159.txt
    | ID_1160.txt
    | ...
    | ...
```

### Train from scratch
* Use Bidirectional LSTM as training model
* Change the path of ```train_dir_path```, ```test_dir_path``` and ```valid_dir_path```
* Run all cells in ```CT05_Case_1.ipynb```
*hyperparameters are set at section ```Set up Bidirectional LSTM model``` in notebook file*

### Download Pretrained models
* Download pretrained models from this url: https://drive.google.com/file/d/1siJCaIpNX5DGxSBP6KaHbogc1ucL-HCc/view?usp=sharing
* Run cells in ```CT05_Case_1.ipynb``` without running the **Start Training** part

### Inference
To inference the trained model, simply run ```CT05_Case_1.ipynb``` without running the **Start Training** part

