# AppContainerPos

- 說明 app Container 位置

---

## 大綱

- [AppContainerPos](#appcontainerpos)
  - [大綱](#大綱)
  - [Simulator (模擬器) 位置](#simulator-模擬器-位置)
  - [iPhone (實體機) 位置](#iphone-實體機-位置)

---

## Simulator (模擬器) 位置

- app 安裝於模擬器，mac 的檔案位置

  > ~/Library/Developer/CoreSimulator/Devices

  - [iphone - Is there any way to see the file system on the iOS simulator? - Stack Overflow](https://stackoverflow.com/questions/6480607/is-there-any-way-to-see-the-file-system-on-the-ios-simulator)

- 找尋對應模擬器的位置

  - 開啟 Xcode 上方選單 [Windows]/[Devices and Simulators]

    ![Devices and Simulators](./pics/2020-05-28-15-39-21.png)

  - 找尋安裝 app 所在的 simulator 版本

    ![Finde simulator ID](./pics/2020-05-28-15-43-37.png)

  - 接下來可以找尋所安裝的 app 本地儲存區塊

    ![Find app container @ Simulator](./pics/2020-05-28-15-51-16.png)

> 可能用程式碼，dump document path 會比較快 (哈)

---

## iPhone (實體機) 位置

- 一樣回到 Xcode 的 [Devices and Simulator] 畫面

- 點選 Device 分頁

  ![Find app container @ Devices](./pics/2020-05-28-15-59-37.png)

- 需注意的是，非 AppStore 安裝的才能看到，一般是 Development 自行安裝才能看到

- 可直接下載及取代，除錯本地檔案時還蠻方便的

---

[=> Top](#appcontainerpos)

[=> Go Back](../README.md)
