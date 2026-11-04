# M3｜Eigenmode 與模態辨識
先完成 M1，並理解線性 LC 模型。

## 到哪裡學
- [4.02 Eigenmode and EPR analysis](https://qiskit-community.github.io/qiskit-metal/tut/4-Analysis/4.02-Eigenmode-and-EPR.html)：eigenmode 設定、場與 EPR 的學習入口。
- [Metal 官方課程目錄](https://qiskit-community.github.io/qiskit-metal/tut/)：延伸閱讀 4.12 Analyzing and tuning a resonator。

## 題目
1. 先求單一 resonator 的目標模式；說明預期是 λ/4、λ/2 或其他結構，並作頻率量級估計。
2. 加入 transmon，明確指定 JJ 的線性 L/C 模型，尋找至少三個 modes。
3. 以 E/H 場分布辨識 qubit-like、resonator-like 或其他模式。模態標籤不可只用排序編號。
4. 掃 resonator 長度為基準的 95%、100%、105%，追蹤同一模態並解釋頻率趨勢。
5. 掃 LJ 為基準的 80%、100%、120%，比較哪些模態較敏感。
6. 至少比較三組網格與兩種 airbox 大小，討論邊界對結果的影響。

## 繳交
模態頻率表、附標籤的場圖、兩組參數掃描、mesh／box 比較、材料與邊界及 junction 設定。

## 驗收與口試
教學起始門檻：solver 收斂，目標模式最後兩組細化頻率差小於 0.1%；若研究目標比此誤差更小，需自行收緊。
- 兩個模式接近或交換排序時，要如何追蹤？
- 線性本徵頻率與 transmon f01 是否相同？
- 無耗散 eigenmode 能否直接提供非諧性、ZZ 或 loaded linewidth？請說明還需哪些模型與分析。

