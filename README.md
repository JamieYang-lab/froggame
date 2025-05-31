# froggame
# 青蛙過馬路 Frog Crossing Game

-這是經典的青蛙過馬路，玩家操控青蛙，躲避車子和障礙物，抵達頂端的遊戲，使用C++製作。

---

## 遊戲玩法

- 使用 **方向鍵** 控制青蛙（F）上下左右移動
- 避開車輛（C）與障礙物（#）
- 成功從底部走到最上方即獲勝
- 撞到車子則遊戲失敗
- 挑戰用最少時間抵達最上方，最快用時會被記錄
- 可選擇三種難度：

| 難度    | 地圖高度 | 車子速度（越小越快） |
|--------|----------|----------------------|
| easy   | 10       | 200ms                |
| medium | 20       | 150ms                |
| hard   | 30       | 100ms                |

    
* 在開始時使用輸入選擇難度，有三種難度可以選，easy高度為10，medium高度為20，hard高度為30。同時車子速度也會加快。<br>
<img src="https://github.com/JamieYang-lab/froggame/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202025-05-28%20185413.png" width="300"/><br>
* 使用方向鍵來操控代表青蛙的F，躲過代表車子的C。O則代表障礙物，車子可以穿越但是青蛙會被阻擋。<br>
<img src="https://github.com/JamieYang-lab/froggame/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202025-05-28%20185849.png"/><br>
* 當青蛙與車子相撞(位置重疊)，會在原地生成X，並且結束遊戲。按enter可以重新開始遊戲，esc則跳出遊戲<br>
<img src="https://github.com/JamieYang-lab/froggame/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202025-05-28%20190225.png" width="300"/><br>
* 當成功操控青蛙到最上端時，跳出遊戲並且顯示成功，同時顯示到達頂端的用時和目前最快成績。如果比之前成績快，則顯示突破紀錄，並且記錄最好成績。<br>
<img src="https://github.com/JamieYang-lab/froggame/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202025-05-28%20190435.png" width="300"/><br>
---

##  專案架構
frog_game/<br>
├── CMakeLists.txt<br>
├── main.cpp<br>
├── Map/<br>
│ ├── Map.h<br>
│ ├── Map.cpp<br>
├── Object/<br>
│ ├── frog.h<br>
│ ├── frog.cpp<br>
│ ├── car.h<br>
│ ├── car.cpp<br>

## 🛠 編譯與執行（CMake + Visual Studio Code）

###  安裝需求

- C++17 編譯器（如 g++, MSVC）
- CMake 3.16+
- Windows 平台（需支援 `<conio.h>`）
- Visual Studio Code + CMake Tools 擴充套件（建議）

###  編譯流程

```bash
# 建立 build 資料夾
mkdir build
cd build

# 執行 CMake 配置與編譯
cmake ..
cmake --build . --config Debug



