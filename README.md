# BSP Hub 使用指南

BSP Hub 提供各種產品系列的 BSP (Board Support Package) Image，檔案結構採用以下層級架構：

## 檔案結構說明

```
產品系列/
    └── 產品型號/
        └── 版本號_作業系統/
            ├── BSP.tgz 或 BSP.tbz2 (BSP 壓縮檔)
            ├── ReadMe.md (安裝與使用說明)
            └── TestReport.pdf (測試報告)
```

### 結構說明
1. 第一層：產品系列名稱
   - 例如：EPC-R7300、MIC-733-AO 等
   
2. 第二層：具體產品型號
   - 例如：EPC-R7300IT-ALA1NN、MIC-733-AO5A1 等
   
3. 第三層：版本號與作業系統資訊
   - 格式：[版本號]_[作業系統]
   - 例如：1.0.0_Ubuntu20、2.0.0

### 如何尋找所需的 BSP Image

1. 確認您的產品系列
   - 從第一層找到您的產品系列名稱（如 EPC-R7300 或 MIC-733-AO）

2. 選擇具體產品型號
   - 進入產品系列資料夾，選擇您的具體產品型號

3. 選擇適合的版本
   - 進入產品型號資料夾，根據版本號和作業系統需求選擇對應的版本資料夾
   
4. 下載所需檔案
   - BSP.tgz 或 BSP.tbz2：BSP 映像檔
   - ReadMe.md：包含安裝步驟和使用說明
   - TestReport.pdf：提供測試報告和相容性資訊

## 範例

如果您需要 EPC-R7300IT-ALA1NN 的 Ubuntu 20.04 BSP：
1. 進入 EPC-R7300 資料夾
2. 選擇 EPC-R7300IT-ALA1NN 資料夾
3. 進入 1.0.0_Ubuntu20 資料夾
4. 下載需要的檔案（BSP.tgz、ReadMe.md、TestReport.pdf）

## 注意事項

- 請確保使用正確版本的 BSP Image
- 安裝前請詳細閱讀 ReadMe.md 文件
- 建議參考 TestReport.pdf 確認硬體相容性