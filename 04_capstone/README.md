# 04｜整合專題：幾何到量子行為
目的：自行連結前面學到的工具，完成一個有參數來源與誤差證據的模擬問題。

## 基本題：Transmon 與讀出 Resonator
1. 選定論文中的一個設計問題，或由講師指定 f01、EC、fr、linewidth 目標。
2. 自行建立 Metal 幾何，取得 C 與 EC，說明 EJ／LJ 的來源。
3. 求 eigenmode 與 S21，辨識目標模態及 loaded linewidth，解釋損耗模型。
4. 根據取得的參數建立合適的 QuTiP 模型，完成 spectrum 或 pulse 分析。
5. 選一個幾何參數做至少三點掃描，解釋它如何改變電路參數及最終預測。
6. 回答：哪些量來自真實求解、哪些是文獻、哪些是你自行假設？對預測有什麼影響？

## 進階題：雙 Qubit／Coupler 的 ZZ
另建雙 qubit 或 qubit–coupler–qubit 設計，取得對應電路參數，說明由電路到耦合 Hamiltonian 的過程，再計算 spectrum 與 ZZ。選一個低混合工作點，以 conditional phase 演化交叉驗證。

請特別說明互電容如何進入耦合模型，不可將 fF 數字直接當成 MHz 的 g；也不可直接把 readout κ 當 qubit 的 1/T1。

## 到哪裡學
回到 [Metal 課程](https://qiskit-community.github.io/qiskit-metal/tut/) 的電容、EPR、coupled-transmon 與 reference designs，以及 [QuTiP 官方文件](https://qutip.readthedocs.io/en/stable/) 的 tensor、eigenstates 與 dynamics 章節。學員需在報告指出採用了哪些段落與近似。

## 繳交
一頁問題說明、電路與幾何、參數來源表、solver 設定與原始結果、量子模型、最終圖與收斂、物理解釋及未解決問題。程式與操作由學員自行完成。

無 solver 時可先做「數值專題」，但須將電磁模擬部分標為未驗收；假設參數不得稱為設計抽取結果。

