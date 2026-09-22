# Zen Sidebar Bookmarks

[English](README.md) | [正體中文](README.zh-TW.md)

A CSS module that allows you to display the Bookmarks Toolbar in the Zen Browser sidebar.

![Preview](assets/preview0.png)

## 📦 Installation

1. Download this repository.
2. Locate the `chrome` directory inside your user profile folder.
3. Place the `userChrome.css` file and the `mods` folder into the `chrome` directory.
4. Restart your browser.

## ✏️ Usage

1. Right-click on the toolbar and select `Customize Toolbar...`.
2. Drag and drop the `Bookmarks toolbar items` above the middle section of the sidebar.
3. Click `Done` in the bottom right corner to save your changes.

> [!NOTE]
> It might be tricky to drag it into the exact position on the first try. You can drag it into the section first and then adjust it upward. Give it a few tries!
> 
> If the `Bookmarks toolbar items` button disappears, simply switch to another tab and back, or reopen the `Customize Toolbar...` page to restore it.

![Customize Toolbar Preview](assets/preview1.png)

## ⚙️ Additional Options

Here are some options you can customize to suit your preferences.

The setup is simple: open `about:config`, create the corresponding preference, and set it to `true`. To disable an option, either set it to `false` or simply remove the preference.

- **Hide folder icons:** Useful if you use emojis as folder names and prefer a cleaner look.

   ```
   zen.sidebar.bookmarks.hide-folder-icon
   ```

   ![Hide Folder Icons Preview](assets/preview2.png)

- **Show overflow menu:** Useful if you have many folders and want items that don't fit in the available sidebar width to be moved into the overflow menu.

   ```
   zen.sidebar.bookmarks.overflow
   ```

   When enabled, the bookmarks toolbar is left-aligned, and items that exceed the available sidebar width are moved into the overflow menu.

## 😞 Known Limitations

- When switching workspaces, the Bookmarks Toolbar may flicker very briefly as it is repositioned. I haven't found a way to fix this yet.
- Dragging items other than the Bookmarks Toolbar into this area is not recommended, as it may cause visual glitches.
- High likelihood of incompatibility with other CSS modules that utilize this same area.

## ❓ Not Working?

- Ensure that `userChrome.css` support is enabled in Zen Browser:

   1. Open the `about:config` page.
   2. Search for `toolkit.legacyUserProfileCustomizations.stylesheets` and toggle it to 	`true`.

- Make sure you placed the files in the correct user profile folder:

   1. Type `about:support` in the address bar and press Enter. 
   2. Look for the Application Basics section.
   3. Click on Open Profile Folder. This will open the folder where Zen Browser stores your user data.

> The above steps are adapted from Zen's Documentation: [Live Editing Zen Theme](https://docs.zen-browser.app/guides/live-editing)

## 📄 License

This project is open-source under the terms of the MIT License.
