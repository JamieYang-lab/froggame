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
  - `easy`：地圖小、車速慢
  - `medium`：標準難度
  - `hard`：地圖大、車速快
    

---

##  專案架構
frog_game/
├── CMakeLists.txt
├── main.cpp
├── src/
│ ├── Map.cpp
│ ├── Car.cpp
│ ├── Frog.cpp
├── include/
│ ├── Map.h
│ ├── Car.h
│ ├── Frog.h


