# ffi Segmentation fault on M1 macOS Big Sur

---

## 大綱

- [ffi Segmentation fault on M1 macOS Big Sur](#ffi-segmentation-fault-on-m1-macos-big-sur)
  - [大綱](#大綱)
  - [說明](#說明)
  - [參考](#參考)

---

## 說明

在執行 pod update 過程，有說明到需要安裝 ffi，

當時的 ffi 版本是對應 1.15.0。

一開始執行 log 建議的 command line 時，還是出現失敗。

- gem pristine ffi --version 1.15.0

  - command line :

    ```sh
    sudo gem pristine ffi --version 1.15.0
    ```

  當時執行後還是失敗。

- gem install --user-install ffi -- --enable-libffi-alloc
  
  上面的執行失敗後，另外在這篇文章 [Segmentation fault on M1 macOS Big Sur · Issue #864 · ffi/ffi · GitHub] 有找到相關的問題，

  看來是 mac M1 macOS Big Sur 的問題，

  裡頭有個解法，有人成功解決，

  - command line :

    ```sh
    gem install --user-install ffi -- --enable-libffi-alloc
    ```

  嘗試後沒，沒有再出現 ffi 的錯誤訊息了，所以關於 ffi 的問題算是解了。

---

## 參考

- [Segmentation fault on M1 macOS Big Sur · Issue #864 · ffi/ffi · GitHub]

---

<!-- 連結設定 -->
[Segmentation fault on M1 macOS Big Sur · Issue #864 · ffi/ffi · GitHub]:
  https://github.com/ffi/ffi/issues/864

[=> Top](#ffi-segmentation-fault-on-m1-macos-big-sur)

[=> Go Back](../README.md)
