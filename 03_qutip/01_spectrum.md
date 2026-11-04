# Q1｜Spectrum 與 Avoided Crossing
## 到哪裡學
- [QuTiP Basic Operations](https://qutip.readthedocs.io/en/stable/guide/guide-basics.html)：查閱 eigenenergies／eigenstates 與態投影。
- [QuTiP Tensor Products](https://qutip.readthedocs.io/en/stable/guide/guide-tensor.html)：建立複合系統。
- 延伸：[Metal Transmon Analytics](https://qiskit-community.github.io/qiskit-metal/tut/4-Analysis/4.32-Transmon-analytics-HCPB.html)，理解電路模型與能譜。

## 教學模型與參數
以兩個 Duffing transmons、交換耦合 RWA 為指定模型。學員需自行寫出並解釋 Hamiltonian。
- f1 = 5.0 GHz，f2 掃 4.4–5.7 GHz，至少 201 點。
- alpha1 = −0.25 GHz，alpha2 = −0.28 GHz。
- 交換項在 H/h 中的係數 g = 0.020 GHz。
- 每個 transmon 先保留 4 個能階，再檢查其他截斷。

## 題目
1. 先求單一 transmon 的低能階與躍遷頻率，驗證參數定義。
2. 建立兩個 transmons 的複合 Hilbert space，掃 f2，畫出相對基態的低能譜。
3. 標示單激發 avoided crossing，比較 g = 0、10、20 MHz。
4. 用 bare-state overlap 說明模式混合；指出按能量排序與按態特徵標籤的差別。
5. 比較每系統 N=3、4、5 時所關心能階的變化，說明此模型下的收斂範圍。
6. 選擇一個驅動算符，討論哪些躍遷可能亮或暗。此題至少交概念說明，進階可計算矩陣元。

## 繳交與驗收
Hamiltonian、單位轉換、能譜圖、bare overlap 圖、耦合與截斷比較。g=0 時應回到獨立系統的可解極限。

口試：Hamiltonian 本徵值圖與實驗吸收譜差在哪裡？看到能階差就一定看到光譜峰嗎？

