# 超導量子晶片 Tutorial｜學習指引與作業
這套教材提供「到哪裡學、學完要完成什麼、如何驗收」。學員自行閱讀官方教材、建立模擬與解釋結果；本資料夾只提供教學文件與題目，不提供實作程式、Notebook 或解答。

## 三個主軸
| 主軸 | 學習內容 | 入口 |
|---|---|---|
| 論文導讀 | 研究問題、模型、關鍵圖與討論；由授課者自行填寫內容 | [論文導讀](01_paper_reading/README.md) |
| 晶片設計 | Qiskit Metal layout、電容與 EC、eigenmode、S21 與 linewidth | [晶片設計](02_chip_design/README.md) |
| 量子模擬 | QuTiP spectrum、ZZ strength、time-domain pulse | [QuTiP](03_qutip/README.md) |

## 建議順序
1. [課前準備](00_setup/README.md)：自行完成官方安裝與基本操作。
2. [論文導讀模板](01_paper_reading/paper_template.md)：由授課者指定論文範圍與內容。
3. Metal 四題：layout → EC → eigenmode → linewidth。
4. QuTiP 三題：spectrum → ZZ → pulse。
5. [整合專題](04_capstone/README.md)：建立有參數來源的幾何到量子模型連結。
6. 依 [評分規準](05_assessment/rubric.md) 與 [報告模板](05_assessment/report_template.md) 繳交與驗收。

## 建議課程安排
| 次數 | 主題 | 主要成果 |
|---|---|---|
| 1 | 論文與先備知識 | 論文導讀、符號與假設表 |
| 2 | Metal layout | 可重建設計、尺寸表 |
| 3 | 電容矩陣與 EC | 節點圖、EC 與收斂 |
| 4 | Eigenmode | 場型辨識、頻率與收斂 |
| 5 | S21 與 linewidth | 複數資料、擬合與誤差 |
| 6 | Spectrum 與 ZZ | 能譜、態標籤、ZZ 曲線 |
| 7 | Time-domain pulse | population、校準與 leakage |
| 8 | 整合專題 | 參數來源與物理解釋 |

每次約 2–3 小時，另留自學與電磁求解時間；可依學員程度拆成更多次。

## 資料夾
- `00_setup`：官方學習入口、先備要求、單位。
- `01_paper_reading`：授課者填寫的導讀與重現模板。
- `02_chip_design`：四項 Metal／電磁模擬作業。
- `03_qutip`：三項 QuTiP 作業。
- `04_capstone`：整合題。
- `05_assessment`：評分與繳交格式。
- `references`：官方資料索引。

根目錄原有博士論文 PDF 保留原位，尚未替它編寫內容或預設授課章節。官方連結核對日期為 2026-11-04；不同版本的章節與 API 可能不同，以學員實際環境記錄為準。


# SQC-toturial
