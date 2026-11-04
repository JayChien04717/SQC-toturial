# M2｜從電容矩陣取得 Charging Energy
先完成 M1。建議時間：自學 2 小時、實作 3 小時，另計求解時間。

## 到哪裡學
- [4.01 Capacitance matrix and LOM analysis](https://qiskit-community.github.io/qiskit-metal/tut/4-Analysis/4.01-Capacitance-and-LOM.html)：Q3D、矩陣與 lumped-element model。
- [4.32 Transmon Analytics](https://qiskit-community.github.io/qiskit-metal/tut/4-Analysis/4.32-Transmon-analytics-HCPB.html)：將電路參數與 transmon 能譜連結。

閱讀後應能解釋 Maxwell／mutual capacitance、reference ground、有效電容及 EC/h 的意義。

## 題目
1. 用自己的 transmon 設計取得電容矩陣，畫出節點與 ground 對應圖。
2. 說明輸出的矩陣種類與單位；檢查對稱性、符號與是否包含參考 ground。
3. 根據裝置的接地或浮接拓樸，推導所需的有效電容與 EC/h；寫明其他節點的邊界條件，不得任取一個對角元素。
4. 重做 M1 的三組 pad width，其他求解設定固定，比較 EC/h 的變化。
5. 至少做三組網格精度，檢查最後關心的 EC 是否收斂。
6. 在指定或自行選定且有來源的 EJ 下，估計 qubit 頻率與非諧性，說明使用的近似及適用範圍。

## 繳交
原始 C 矩陣、節點示意圖、EC 推導、尺寸對 EC 圖、網格對 EC 圖、solver 設定與參數來源。

## 驗收與口試
教學起始門檻：solver 達自身收斂條件，且最後兩組細化 EC 相對差小於 1%；若未達到，應指出原因並提出改進。
- 哪些條件下單一總電容模型合理？
- 浮接兩島與單島接地的處理差在哪裡？
- 只知道 C，能否唯一決定 transmon 頻率？還缺什麼？

