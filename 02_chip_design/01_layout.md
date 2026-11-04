# M1｜建立並修改晶片 Layout
建議時間：自學 2 小時、實作與討論 2–3 小時。

## 到哪裡學
1. [1.1 Quick start](https://qiskit-community.github.io/qiskit-metal/tut/1-Overview/1.1-Quick-start.html)：設計、元件與 GUI。
2. [2.12 Simple Meander](https://qiskit-community.github.io/qiskit-metal/tut/2-From-components-to-chip/2.12-Simple-Meander.html)：CPW 路由與長度參數。
3. [3.3 Render to Ansys](https://qiskit-community.github.io/qiskit-metal/tut/3-Renderers/3.3-Render-your-design-to-Ansys.html)：幾何如何交給電磁求解器。

先理解：design／component／pin 的關係、幾何單位、signal 與 ground、加法與扣除幾何。

## 題目
1. 自行完成一個 transmon 與一個 CPW resonator 的 layout，說明各部分用途。
2. 選一種 transmon 元件，將其 pad width 設為 350、425、500 μm，其餘參數固定；若該元件不適用這些尺寸，提出替代值並說明理由。
3. 將 resonator 電氣路徑長度改為基準的 95%、100%、105%，檢查路由是否仍正確。
4. 指出 JJ、兩側導體、coupling gap、ground 與預計求解的區域。
5. 說明此結構是否已具備量測 S21 所需的 feedline 與 ports；若沒有，提出 M4 要補的結構。

## 繳交
基準與變化設計截圖、尺寸對照表、可重建設計檔，以及一頁「改動前的物理預測」。

## 驗收與口試
- 能從設定重新產生設計，並指出實際改變了哪個尺寸。
- 能檢查短路、斷線、路由穿越與超出 chip 範圍。
- 回答：幾何路徑長度與電氣長度為什麼未必完全相同？
- 回答：畫出 JJ 與指定其電磁模型，分別完成了什麼工作？

