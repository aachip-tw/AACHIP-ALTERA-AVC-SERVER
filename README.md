# AACHIP-ALTERA-AVC-SERVER
AACHIP Altera XVC Server，透過網路提供 JTAG 存取服務，用於 Altera／Intel FPGA 的遠端除錯與開發。
# AACHIP-ALTERA-AVC-SERVER

AACHIP Altera XVC Server（AVC）提供網路至 JTAG 的存取服務，讓相容的用戶端透過 TCP/IP 連接伺服器端的 Altera／Intel FPGA 硬體。

XVC 為 Xilinx Virtual Cable 協定；本專案將其應用於 Altera FPGA 的 JTAG 存取。實際支援的操作取決於伺服器、JTAG 介面及用戶端工具的相容性。

## 應用情境

- 透過區域網路存取遠端 FPGA 的 JTAG 介面。
- 將 FPGA 板卡與開發端電腦分開放置。
- 配合相容工具進行硬體開發、測試與除錯。

## 軟體下載

請前往本儲存庫的 **Releases** 頁面下載安裝包，並閱讀對應版本的發布說明。

## 基本使用流程

1. 在連接 FPGA 硬體的電腦上安裝 AVC Server。
2. 安裝對應的硬體驅動，並確認 JTAG 接線與供電。
3. 啟動伺服器，依軟體介面設定監聽位址及 TCP 連接埠。
4. 在相容的 XVC 用戶端設定伺服器 IP 與連接埠。
5. 建立連線後，依工具支援範圍執行 JTAG 操作。

## 使用注意事項

- 支援的 FPGA、USB／JTAG 介面、用戶端及操作方式，以各版本說明為準。
- XVC 協定本身不提供身分驗證或傳輸加密，建議在可信任的區域網路或 VPN 內使用。
- 若無法連線，請檢查伺服器狀態、IP、連接埠及防火牆設定。

## 技術支援

合合科技有限公司  
https://aachip.com.tw/

回報問題時，請提供軟體版本、FPGA／JTAG 介面型號、用戶端工具及錯誤訊息。
