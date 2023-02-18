## 前言
  最近在學習chatGPT API的Embedding時遇到了一段沒看過的指令
  ```
  D:your-file-path>python -m venv env
  ```
  原來是建立虛擬環境的意思，就順便把github當blog紀錄一下

## 步驟

### 建立擬環境
  ```
  python -m venv env
  ```
  - -m : 命令行選項，代表要執行的模組 \
  - venv : 是一個python內建模組，用於建立虛擬環境，是一個獨立的副本，能夠在同一台電腦上面建立多個python項目，每個項目都擁有一組依賴的套件  \
  - env : 建立一個名為「env」的虛擬環境 \
  \
  原來這樣建立後每個套件都不會互相影響拉~ cool \
  \
  建立好後就會出現env資料夾 \
  ![image](https://user-images.githubusercontent.com/84761318/219600906-24961f87-6ba3-44a7-b4d2-365d1d4aef69.png)

### 啟動虛擬環境
  ```
  D:your-file-path>env/bin/activate
  ```
  啟用後在開頭的提示符會顯示`(env)...` \
  此時就切換成虛擬環境 \
  ![image](https://user-images.githubusercontent.com/84761318/219605440-7c820abf-fb5e-4dcb-9b47-3da4f6c34da1.png)
  
### 安裝套件
  目前套件有以下數量 \
  ![image](https://user-images.githubusercontent.com/84761318/219827241-6d224d45-98d1-4029-aa74-9ec32b8cb5aa.png)
  安裝requirements.txt內所需的套件 \
  ```
  python -m pip install -r requirements.txt
  ```  
  我有發現原本沒有輸入`python -m`的話會出現權限問題，而無法順利安裝(原因不得而知，如果有了解的朋友可以提市就太感謝了) \
  \
  安裝完後的套件數量: \
  ![image](https://user-images.githubusercontent.com/84761318/219828655-e09367f3-7912-4cf8-a5dd-3866ea10183f.png)
  這樣就成功已虛擬環境進行測試了 \
### 退出虛擬環境
  ```
  deactivate
  ```
  如果沒有使用的話需要到工作管理員中關閉喔~
