# Q2｜靜態 ZZ Strength
先完成 Q1，沿用相同模型與參數。

## 到哪裡學
- [QuTiP Basic Operations](https://qutip.readthedocs.io/en/stable/guide/guide-basics.html)：eigenstates、overlap 與 expectation。
- [QuTiP Tensor Products](https://qutip.readthedocs.io/en/stable/guide/guide-tensor.html)：複合基底及算符。
- [QuTiP Master Equation Guide](https://qutip.readthedocs.io/en/stable/guide/dynamics/dynamics-master.html)：延伸題的時間演化。

這些官方章節教的是工具。ZZ 的模型與態標籤需要學員自己組合，不預設官網提供完全相同的現成範例。

## 題目與定義
本作業定義 ζ = (E11 − E10 − E01 + E00)/h，以 MHz 回報。Eij 指與 bare |ij〉對應的 dressed energy，如何建立對應也是本題的一部分。
1. 自行提出一致的四態指派規則，避免同一本徵態被配給兩個標籤。
2. 掃 f2，繪製 ζ 與四個 dressed-state overlaps。
3. 指出 |11〉與 |20〉／|02〉強混合區，說明何時 computational-state ZZ 的解讀不再穩健。
4. 比較 g=0、10、20 MHz，在遠離共振的工作點討論趨勢。
5. 比較 N=2、3、4、5，解釋高能態對 ZZ 的影響與模型限制。
6. 選一個低混合工作點，討論 ζ 與有效 Z⊗Z 項係數、條件頻移的關係，明確定義 Z 與 2π convention。

## 延伸題
用兩種控制 qubit 初態進行 conditional Ramsey，從相位隨時間的變化估計 ZZ，與本徵能量差比較。若直接交換仍明顯，需說明如何分離 population dynamics 與相位。

## 繳交與驗收
ZZ 掃描、四態標籤與 overlaps、零耦合極限、截斷比較、一個工作點的解釋。不得只用排序後第幾個能量直接指定 E11。

口試：ζ 在某處突然跳變，如何判斷是物理現象、態標籤切換，還是數值問題？

