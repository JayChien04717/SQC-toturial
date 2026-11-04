# 求解前準備與共同紀錄
請先完成官方 [Render to Ansys](https://qiskit-community.github.io/qiskit-metal/tut/3-Renderers/3.3-Render-your-design-to-Ansys.html)，再依 M2–M4 的指定教材完成各自求解。此文件是待完成清單，操作方法由學員閱讀官方文件學習。

## 求解前
- 說明選用 Q3D、HFSS 或其他求解器的理由及可取得的物理量。
- 記錄 Metal、renderer、AEDT／solver 與 OS 版本，確認授權。
- 核對幾何單位、基板材料、金屬、ground 連通性、signal nets 與耦合間隙。
- 說明 junction 在靜電與 eigenmode 模型中的不同處理方式。
- 指出 ports、open／short terminations、邊界及 airbox 的位置。

## 求解後
- 保存原始 project 或可重建檔，及所有非預設設定。
- 電容：記錄節點順序、矩陣種類、參考 ground 與單位。
- Eigenmode：保存頻率、場圖、模態標籤與每次網格結果。
- S21：保存複數原始資料、掃頻設定、校準方式與擬合殘差。
- 記錄成功與未成功的收斂檢查，提出下一步改進。

口試：另一位同學能否僅依你提交的設定重建相同問題？如果不能，缺少哪項資訊？

