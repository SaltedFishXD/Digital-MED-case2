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


下載TrainingData.zip並解壓縮後，使用以上環境，
* Case2.ipynb
    * 資料讀取&整理
        * 利用pydicom讀取資料將data轉為narray存取，並透過openCV將圖形收縮至固定大小後，進行鏡像翻轉(左右、上下)與角度旋轉增加訓練
        * 讀取資料 : 
![image](https://github.com/SaltedFishXD/Digital-MED-case2/blob/main/loadFile.png)
    * use_bag_of_word_and_machine_learning.ipynb
        * 使用bag of word選取有關鍵字的句子，並用有關鍵字的句子做機器學習，使用trainset的資料做train test split(比例7:3) 做出來的accuracy可達0.9。而程式後半部測試學校給予的testset，但不知道的每個txt file的true label，所以輸出僅輸出預測結果。下面圖片是輸出結果

![image](https://github.com/SaltedFishXD/Digital-MED-case2/blob/main/loadFile.png)

