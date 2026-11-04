# 00｜課前準備與自學方式
## 先備知識
學員應先具備基本線性代數、LC 電路、量子態與算符、複數數據及基本程式操作能力。遇到安裝問題先閱讀官方文件，並記錄錯誤、版本與嘗試過的方法。

## 指定官方入口
- [Qiskit Metal／Quantum Metal 官方首頁](https://qiskit-community.github.io/qiskit-metal/)：由 Get Started → Installing 與 Choose Your Path 開始。
- [Metal 官方課程](https://qiskit-community.github.io/qiskit-metal/tut/)：先完成 Part 1，再讀 Part 2 的元件、pin 與 routing。
- [QuTiP 官方文件](https://qutip.readthedocs.io/en/stable/)：先讀 Installation，再讀 Users Guide。
- [QuTiP Basic Operations](https://qutip.readthedocs.io/en/stable/guide/guide-basics.html)：理解 Qobj、態、算符、expectation 與 eigenstates。
- [QuTiP Tensor Products](https://qutip.readthedocs.io/en/stable/guide/guide-tensor.html)：理解多系統算符與子系統順序。

## 課前任務 P0
1. 依官方說明完成環境，記錄 OS、套件與 solver 版本。
2. 自行完成一個 Metal 官方入門範例；指出一個元件、一個 pin 與一個幾何參數。
3. 自行完成一個 QuTiP 官方基本操作範例，說明態、算符與 expectation 的差別。
4. 確認實驗室是否有可用 Q3D／HFSS 與授權，或由講師指定其他求解器。
5. 閱讀 [單位約定](units.md)，列出自己最容易混淆的兩組單位。

繳交：一頁環境紀錄、官方教材連結、完成畫面及遇到問題的處理紀錄。驗收重點是能說明自己的操作，不是只有安裝成功截圖。

## 軟體分工
Metal 用於幾何設計與串接分析；電容及全波模擬還需對應求解器。QuTiP 用於建立量子模型及其動力學。未取得電磁求解資源時可先完成 QuTiP 作業，電磁部分另安排驗收。版本與 renderer 的選擇依官方文件及實驗室可用環境決定。

