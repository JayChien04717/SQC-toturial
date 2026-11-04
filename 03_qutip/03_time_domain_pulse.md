# Q3｜Time-domain Pulse、Leakage 與耗散
## 到哪裡學
- [Lindblad Master Equation Solver](https://qutip.readthedocs.io/en/stable/guide/dynamics/dynamics-master.html)：初態、演化與 expectation。
- [Time-dependent Hamiltonians](https://qutip.readthedocs.io/en/stable/guide/dynamics/dynamics-time.html)：時間相依驅動。
- [Solver API](https://qutip.readthedocs.io/en/stable/apidoc/solver.html)：查閱容差、內部步長與結果儲存。

## 教學設定
單 transmon，f01=5.0 GHz，alpha=−0.25 GHz，先保留 3 個能階，以 |0〉為初態。可用 rotating frame + RWA，但需自行寫出 frame、detuning 與 amplitude convention。

耗散比較設定：T1=30 μs、Tphi=50 μs。時間軸統一用 ns，學員需推導 collapse operators 並檢查 0–1 coherence 的衰減定義。

## 題目
1. 建立 resonant square pulse，掃脈衝時間或幅度，觀察 Rabi oscillation。
2. 改成 Gaussian pulse：sigma=10 ns，中心 40 ns，模擬區間 0–80 ns。自行估計初始幅度，再掃幅度校準。
3. 畫 envelope 及 P0、P1、P2；同時回報最大暫態 P2 與脈衝後 residual P2。
4. 選 sigma=5、10、20 ns 做比較；調整時間窗口以涵蓋各脈衝，並各自重新校準。
5. 比較無耗散與指定 T1/Tphi 的結果，分別解釋能量鬆弛與純退相干。
6. 比較 N=3、4、5，並收緊 ODE 容差及最大步長，說明結果是否穩定。僅增加繪圖取樣點不算積分收斂檢查。
7. 回答：最高末態 P1 能否代表完整單 qubit gate fidelity？還缺少哪些測試？

## 繳交與驗收
Hamiltonian、pulse 定義、幅度校準曲線、population、leakage、耗散與數值收斂比較。population 總和應在數值誤差內為 1，並說明是否存在非物理負值。

延伸：自行到官方文件查找適用工具，完成 DRAG、Ramsey／echo 或雙 qubit 條件脈衝中的一題，說明新增的物理因素。

