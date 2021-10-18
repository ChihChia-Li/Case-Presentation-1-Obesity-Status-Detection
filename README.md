# Case-1_Obesity-Status-Detection
## Digital Medicine 2021 

### Basic Requirements
* Python 3.7
* keras

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

### Download Pretrained models
* Download pretrained models from model folder
* Run cells in ```CT05_Case_1.ipynb``` without running the **Start Training** part

### Inference
To inference the trained model, simply run ```CT05_Case_1.ipynb``` without running the **Start Training** part

