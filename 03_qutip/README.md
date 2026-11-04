# 03｜QuTiP 量子模擬
由學員自行學習官方文件並建立模型。此處提供題目、參數與驗收，不提供可直接執行的解答。

## 共同必讀
1. [Basic Operations on Quantum Objects](https://qutip.readthedocs.io/en/stable/guide/guide-basics.html)：Qobj、basis、operators、eigenstates、expectation。
2. [Tensor Products and Partial Traces](https://qutip.readthedocs.io/en/stable/guide/guide-tensor.html)：多 qubit Hilbert space。
3. [Lindblad Master Equation Solver](https://qutip.readthedocs.io/en/stable/guide/dynamics/dynamics-master.html)：封閉與開放系統演化。
4. [Time-dependent Hamiltonians](https://qutip.readthedocs.io/en/stable/guide/dynamics/dynamics-time.html)：脈衝與時間相依係數。

| 題目 | 目標 |
|---|---|
| [Q1：Spectrum](01_spectrum.md) | 建 Hamiltonian、辨識能階、理解 avoided crossing |
| [Q2：ZZ strength](02_zz_strength.md) | 計算條件頻移、追蹤 dressed states、檢查近似 |
| [Q3：Time-domain pulse](03_time_domain_pulse.md) | 觀察 Rabi、校準 pulse、比較 leakage 與耗散 |

建議先做 transmon 的弱非諧模型；若論文使用 fluxonium 或其他器件，另選適合的 Hamiltonian 與基底，不能直接沿用 Duffing transmon 參數。

共同繳交：模型方程、參數與單位、初態、基底與截斷、數值設定、結果圖、物理解釋及參考官方章節。作業的教學參數不是任何晶片的實測值或電磁抽取結果。

