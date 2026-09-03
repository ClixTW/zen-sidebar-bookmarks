# Zen 側邊欄書籤列

[正體中文](README.zh-TW.md) | [English](README.md)

一個允許將書籤列顯示在 Zen 瀏覽器側邊欄的 CSS 模組。

![示意圖](assets/preview0.png)

## 📦 安裝步驟

1. 下載本儲存庫。
2. 找到使用者設定檔中的 `chrome` 目錄。
3. 將 `userChrome.css` 檔案和 `mods` 資料夾放至 `chrome` 目錄中。
4. 重啟瀏覽器。

## ✏️ 使用方式

1. 在工具列點擊右鍵，選擇 `自訂工具列…`。
2. 將 `書籤工作列項目` 拖放到側邊欄的中間區塊上方。
3. 點擊右下角的 `完成` 結束設定。

> [!NOTE]
> 可能不太容易一次就拖放到正確的位置。可以先拖放到該區塊內，再移動到上方，多試幾次！

![自訂工具列示意圖](assets/preview1.png)

## ⚙️ 額外選項

如果想隱藏書籤列上的資料夾圖標，請將 `userChrome.css` 的以下部分取消註解：

```css
@import "mods/hide-bookmark-folder-icons.css";
```

當你使用 Emoji 當作資料夾名稱，希望有更簡潔的顯示效果時，這會有所幫助。

![隱藏資料夾圖標示意圖](assets/preview2.png)

## 😞 已知限制

- 不建議將書籤列以外的按鈕拖放到此區域中，會有一些視覺上的故障。
- 很可能與其他使用此區塊的 CSS 模組不相容。

## ❓ 不起作用？

- 請確定已為 Zen 瀏覽器開啟 `userChrome.css` 支援：

   1. 在網址列輸入 `about:config` 並按下 `Enter`。
   2. 搜尋  `toolkit.legacyUserProfileCustomizations.stylesheets` 並將其切換為	`true`。

- 確定將檔案放入了正確的使用者設定檔：

   1. 在網址列輸入 `about:support` 並按下 `Enter`。
   2. 尋找「應用程式一般資訊」中的「設定檔目錄」項目。
   3. 按下「開啟資料夾」。這將會開啟 Zen 瀏覽器儲存您使用者設定檔的目錄。

> 以上教學來自 Zen 的官方文檔： [Live Editing Zen Theme](https://docs.zen-browser.app/guides/live-editing)

## 📄 License

本專案基於 MIT License 條款開源。
