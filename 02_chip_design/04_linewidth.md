# M4｜S21 與 Resonator Linewidth
先完成 M3。目標是自行選擇合適模型、檢查擬合與數值收斂。

## 到哪裡學
- [4.03 Impedance, admittance and scattering](https://qiskit-community.github.io/qiskit-metal/tut/4-Analysis/4.03-Impedance.html)：driven 模擬與掃頻。
- [4.17 S21 simulation and fitting](https://qiskit-community.github.io/qiskit-metal/tut/4-Analysis/4.17-Fit-S21-of-Hanger-Resonator-Geometry.html)：hanger resonator 與 S21 擬合。

## 題目
1. 建立可量測傳輸的 feedline–resonator 結構，定義兩個 50 Ω ports 與 reference planes。
2. 先粗掃定位 resonance，再自行選擇窄掃範圍與間距，保存複數 S21。
3. 畫出 magnitude、phase 與複數平面圖，判斷是否需要背景、delay 或非對稱修正。
4. 查閱官方範例，選擇擬合模型，取得 resonance frequency、loaded linewidth 與 QL；提供殘差。
5. 說明 linewidth、κ、能量衰減時間與場振幅衰減時間的定義及換算。
6. 將 coupling gap 改為基準的 80%、100%、120%，其他條件固定，比較 linewidth 趨勢；確認沒有造成金屬接觸。
7. 細化 mesh 及掃頻間距，分別檢查 fr 與 linewidth 的穩定度。

## 繳交
完整幾何與 port 設定、原始複數資料、模型與擬合參數、殘差、gap 掃描及收斂比較。

## 驗收與口試
教學起始門檻：linewidth 內至少約 20 個取樣點；solver 收斂，最後兩組細化 linewidth 差小於 5%。有插值掃頻時用局部 discrete sweep 檢查窄峰。
- 複數 notch 擬合出的 linewidth 與圖上直接量 dip 半深寬，是否必然相同？
- Qi、Qc、QL 分別代表什麼？你的模型包含哪些損耗？
- 為什麼本徵頻率收斂，不代表 linewidth 也已收斂？

