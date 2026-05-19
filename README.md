# 圖書管理系統 (Book Management System)

這是一個基於 C# Windows Forms (WinForms) 開發的圖書管理與借閱系統。本專案為視窗程式設計的實作練習，主要展示 `ListView` 控制項的進階應用，包含多種視圖切換、圖文整合顯示，以及與其他控制項的事件連動功能。

## 專案簡介 (Project Introduction)

本程式模擬了一個簡易的圖書借閱介面。使用者可以在左側的 `ListView` 瀏覽館藏書籍，並透過右上角的下拉式選單即時切換不同的檢視模式（如大圖示、詳細資料等）。當使用者找到想借的書時，只需雙擊書籍圖示，系統便會彈出確認視窗，並將確認借閱的書籍自動加入至右側的借書清單中。

### 核心功能特色
* **多視圖動態切換**：整合 `ComboBox` 與 `ListView.View` 屬性，支援 5 種檢視模式：
  * 大圖示 (LargeIcon)
  * 詳細資料 (Details - 顯示書名、作者、類別)
  * 小圖示 (SmallIcon)
  * 清單 (List)
  * 大圖示加詳細資料 (Tile)
* **圖文整合顯示**：利用 `ImageList` (LargeImageList / SmallImageList) 綁定書籍封面圖片。
* **防呆借閱機制**：透過 `ItemActivate` 事件捕捉雙擊動作，並具備重複借閱檢查（若書籍已在清單中則不會重複觸發）。

## 使用技術與控制項 (Technologies & Controls)

* **開發語言**: C#
* **框架**: .NET Windows Forms
* **主要控制項**: 
  * `ListView` (資料展示與事件觸發)
  * `ComboBox` (視圖模式選擇)
  * `ListBox` (借閱清單紀錄)
  * `ImageList` (圖片資源管理)

## 執行說明 (How to Run)

1. **取得專案**：將此儲存庫 (Repository) Clone 到本地端，或下載 ZIP 壓縮檔。
   ```bash
   git clone [https://github.com/Zhang-chen415/1131435_LibraryManagement.git](https://github.com/Zhang-chen415/1131435_LibraryManagement.git)
   ```
2. **開啟專案**：使用 Visual Studio 開啟專案資料夾中的 .sln 解決方案檔。
3. **編譯與執行**：按下 F5 或點擊「開始」即可編譯並執行程式。

## 程式截圖 (Screenshots)

1. 大圖示檢視模式
<img width="1901" height="1058" alt="image" src="https://github.com/user-attachments/assets/fe0e3f99-f31e-4d1f-880d-0dd73006b550" />

2. 詳細資料檢視模式
<img width="1905" height="933" alt="image" src="https://github.com/user-attachments/assets/74d20a9e-dd57-4af4-9774-8a2b9c363399" />



