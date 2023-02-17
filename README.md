## 前言
  最近在學習chatGPT API的Embedding時遇到了一段沒看過的指令
  ```
  D:your-file-path>python -m venv env
  ```
  原來是建立虛擬環境的意思，就順便把github當blog紀錄一下

## 建立虛擬環境
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
