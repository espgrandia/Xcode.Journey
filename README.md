# Xcode 旅程

Xcode 的相關資訊放置於此

---

## Xcode 功能

- [CommandLine 除錯方式](./CommandLineDebug/README.md)
  
  > command line 的帶入參數。

- [App Container 位置](./AppContainerPos/README.md)

  > 說明 app Container 位置

- [使用 Aggregate 來產出 framework](./ExportedFrameworkWithAggregate/README.md)

  > 在 Xcode 專案中，可透過 shell script 來產出 framework 的設定方式。

- [Network Link Conditioner](./Network_Link_Conditioner/README.md)

  > Apple 提供的模擬網路環境的工具， 有 Mac 以及 iPhone 啟用的方式說明。

- [啟用系統監視器](./SystemMonitor/README.md)

  > 如何透過 `系統監視器` 查看 iPhone : Devices，模擬器的 system log。

---

## 送審

- [自動提供 缺少出口合規資訊](./Provided_Automatically_Export_Compliance/README.md)

  > 說明如何在 Info.plist 設定，免除需要交付出口合規文件。

- [Xcode Archive Upload To App Store Connect](./Xcode_Archive_Upload_To_AppStoreConnect_Using_FlutterProject/README.md)

  > 說明 Flutter Project for iOS，
  >
  > 如何透過 Xcode 產生對應的 archive，
  >
  > 並上傳到 App Store Connect。
  >
  > 中間有修正一些客製化的腳本來加速產出。

---

## 障礙排除

- [Xcode10_BuildSystem](./Xcode10_BuildSystem/README.md)

  > 之前舊專案升級到 Xcode 10 時，遇到 Build System 不相容的處理方式。

- [Lost AppleWWDRCA Issue](./Lost_AppleWWDRCA_Issue/README.md)

  > 在新 mac os 環境，匯入開發者憑證，該憑證還在有效期，
  >
  > 但憑證卻為失效狀態的問題排查。

- [Lost AppleWWDRCA Part II Issue](./Lost_AppleWWDRCA_PartII_Issue/README.md)

  > 正常使用一段時間後，新增一個 iOS 的開發者憑證，遇到失效問題。
  >
  > 但原有的是有效的，此為排查原因。

- [CodeSign for Keychain](./CodeSignForKeychain/README.md)

  > 釐清 codesign 詢問 keychain 中的密鑰時機。
