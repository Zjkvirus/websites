# 為何增強模式是必要的？

-----------------------

增強模式提供以下功能：

1. 不再需要依賴 logcat 偵測 app 程序建立
   - 規避由於日誌可能延後而導致有一小段時間應用程式不會被隔離的問題
   - 規避 log 被關閉的問題（如 Huawei EMUI 開機時禁用 log）
2. 開機啟動
   - 規避定製系統禁止開機啟動的問題（包括但不限於 MIUI）
3. 禁止系統重新掛載
   - 規避定製系統的行為觸發重新掛載導致隔離失效（如 MIUI 11）
4. 記錄應用程式訪問檔案行為
4. 修改/修復應用程式的部分行為以保證應用程式功能正常

## 效能影響

「增強模式」只帶來可以忽略不記的效能影響。