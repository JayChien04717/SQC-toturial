# 單位、符號與模型邊界

| 量 | 定義與單位 |
|---|---|
| f、g、alpha、EC/h、EJ/h | GHz，cycles/ns；`g` 是 Hamiltonian 中交換項的係數 |
| H/h | GHz，學員能譜圖使用的能量除以 h |
| H/hbar | rad/ns，與 H/h 相差 2π；需依 QuTiP 的時間演化約定處理 |
| 時間 | ns；30 μs = 30000 ns |
| C | 輸入矩陣 fF，計算 SI 時乘 1e-15 |
| linewidth Δf | 功率 Lorentzian 的 FWHM，GHz |
| κ | 能量衰減率，ns⁻¹；κ = 2πΔf，QL = fr/Δf |
| ζ | `(E11-E10-E01+E00)/h`，GHz；輸出 MHz 時乘 1000 |

對一個單模線性共振器，若能量按 exp(-κt) 衰減，場振幅按 exp(-κt/2) 衰減。不要把兩者的 lifetime 混用。以單光子衰減模型描述時，QuTiP collapse operator 是 `sqrt(κ)*a`。

浮接 transmon：必須先定義兩島的差模電荷與其他節點邊界條件。不能把任意一個 Maxwell 對角元素當成總有效電容。電容矩陣與節點基底改變時，Hamiltonian 也要一起變換。

QuTiP 入門採弱非諧 Duffing transmon、交換耦合 RWA 與有限能階截斷。Duffing 模型不適用於高激發、遠離 transmon regime 或任意 fluxonium。若要延伸 fluxonium，應從 `4EC n² + EL(phi-phi_ext)²/2 - EJ cos(phi)` 的適當基底建立各自的能譜與矩陣元，再投影耦合；不能直接沿用 transmon 的 alpha。

本教材 spectrum 指 Hamiltonian 的能階／躍遷頻率。實驗吸收譜或 QuTiP 的兩時間關聯 `spectrum()` 還牽涉驅動、耗散與選擇定則，不等同於本徵值圖。
