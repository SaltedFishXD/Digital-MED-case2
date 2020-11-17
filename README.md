# 數位醫學 -Case2
### python 環境 
* 環境
    * python                    3.7
    * os(python 內建)
    * re(python 內建)
    * pytorch                   1.2.0 
    * numpy                     1.18.5
    * torchvision               0.8.1
    * torch.utils.data.dataset              
    * matplotlib.pyplot
    * pydicom                   
    * sklearn.model_selection   
    * openCV                    4.4.0
    * cudatoolkit               10.1
    
    
### 使用說明 


下載TrainingData.zip並解壓縮後，使用以上環境(如果要使用GPU請務必至Nvidia官網下在相關CUDA版本，pythorch版本也請自行調整)
p.s cudatoolkit ≠ CUDA
* Case2.ipynb
    * 資料讀取&整理
        * 利用pydicom讀取資料將data轉為narray存取，並透過openCV將圖形收縮至固定大小後，進行鏡像翻轉(左右、上下)與角度旋轉增加訓練
        * 讀取資料 : 
![image](https://github.com/SaltedFishXD/Digital-MED-case2/blob/main/loadFile.png)
    * train & test dataset split 8 : 2 (train_test_split)
    
    
    * CNN Model 架構
        * 利用torch建立本次測驗所需的 kernel size、Convolutional layer、fully connection layer
        * 進行訓練
        
   ![image](https://github.com/SaltedFishXD/Digital-MED-case2/blob/main/CNN-Layer.png)

