# 🔒 潇潇图片混淆 v1.5 - 使用指南 / User Guide

本工具是一款高性能、纯本地运行的批量图片空间重组（混淆/解混淆）工具。支持中文密钥，并提供元数据擦除功能以保护隐私。

This tool is a high-performance, fully local batch image spatial reorganization (obfuscation/de-obfuscation) tool. It supports custom Chinese keys and metadata erasure for privacy protection.

---

## 快速上手 / Quick Start

### 1. 导入图片 / Import Images
你有三种方式将图片导入到工具中：
* **点击或拖拽**：点击页面中央的虚线框，或者将多张图片/ZIP压缩包拖拽到页面中。
* **剪切板粘贴**：在页面任意地方使用快捷键 `Ctrl + V`，可以直接粘贴剪切板中的图片。

There are three ways to import images into the tool:
* **Click or Drag & Drop**: Click the dashed area in the center, or drag and drop multiple images/ZIP files directly into the page.
* **Clipboard Paste**: Press `Ctrl + V` anywhere on the page to paste an image directly from your clipboard.

### 2. 配置选项 / Configuration Settings
在处理图片前，你可以调整以下设置：
* **混淆密码**：在输入框中输入密码（支持中文/字符）。相同的密码才能完美还原图片。如果留空，系统将使用默认常数。
* **导入自动处理设置**：可选择“不自动处理”、“自动混淆”或“自动解混淆”。勾选后，新导入的图片会自动执行相应操作。
* **安全与隐私控制**：勾选“彻底擦除图片元数据”可在上传时清空图片的拍摄地点、设备等 EXIF 信息。

Before processing, you can adjust the following configurations:
* **Obfuscation Password**: Enter a password (supports Chinese/characters). The *exact same password* must be used to revert the image. Leave it blank to use the default constant.
* **Auto-Process Settings**: Choose between "No Auto-Process", "Auto Encrypt", or "Auto Decrypt". If enabled, newly imported images will be processed instantly.
* **Privacy Control**: Check "Thoroughly erase image metadata" to strip EXIF data (such as location, camera model) upon uploading.

### 3. 批量处理与保存 / Batch Processing & Saving
使用功能按钮栏进行快捷操作：
* **全部混淆** 🔒：一键混淆所有导入的图片。
* **全部解混淆** 🔓：一键将所有混淆过的图片尝试还原。
* **全部还原** ↻：放弃当前修改，将所有图片恢复到刚导入时的状态。
* **批量保存** 💾 / **批量分享** 📤：将所有处理后的图片打包成一个 ZIP 压缩包下载或调用系统分享。
* **清空布局** 🗑️：移除当前所有的图片任务。

Use the button group for quick operations:
* **Encrypt All (全部混淆)** 🔒: Obfuscate all imported images with one click.
* **Decrypt All (全部解混淆)** 🔓: Attempt to restore all obfuscated images with one click.
* **Restore All (全部还原)** ↻: Discard current modifications and revert all images to their original uploaded state.
* **Save All (批量保存)** 💾 / **Share All (批量分享)** 📤: Package all processed images into a ZIP file for download or system sharing.
* **Clear All (清空布局)** 🗑️: Remove all current image tasks.

---

## 单张图片控制 / Individual Image Control

每张图片下方都有一组专属按钮，用于单独控制：
* **混淆** / **解混**：单独对该图片进行加密或解密。
* **分享** 📤：在手机端会弹出预览图，**长按图片**即可发送给朋友；在电脑端可**右键另存为**。
* **原图**：将单张图片恢复到初始状态。
* **删除任务**：从列表中移除该图片。

Each image card has its own control buttons underneath:
* **Encrypt (混淆)** / **Decrypt (解混)**: Obfuscate or de-obfuscate this specific image.
* **Share (分享)** 📤: Opens a pop-up window. **Long-press the image** on mobile to send/save it, or **right-click and "Save image as..."** on desktop.
* **Original (原图)**: Revert this single image to its original uploaded state.
* **Remove (删除任务)**: Delete this image from the dashboard.

---

## 💡 重要提示 / Important Notes

> ⚠️ **关于密码 (About Passwords)** > 请务必牢记你加密时使用的密码！如果密码输入错误，或者空格/大小写不一致，解出来的图片将会是一团乱码，无法正常观看。
>
> Please remember the exact password used for encryption! If the password is incorrect (including spaces or case mismatches), the decrypted image will remain scrambled and unviewable.

> 🔒 **隐私安全 (Privacy & Security)** > 本工具完全基于前端 JavaScript 运行，**所有图片处理均在您的浏览器本地完成**，绝不会上传到任何服务器，请放心使用。
>
> This tool runs purely on front-end JavaScript. **All processing happens locally in your browser.** No images or passwords are ever uploaded to any server. Your privacy is 100% secure.

项目参考:https://github.com/jiarandiana0307/PicEncrypt

Project Reference:https://github.com/jiarandiana0307/PicEncrypt
