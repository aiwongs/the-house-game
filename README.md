# The House - 剧情重制 & 中文增强版 (Remastered by aiwongs)

## 📖 项目简介

本项目是基于 Artur Kot 的原创冒险游戏 [The House](https://github.com/arturkot/the-house) 进行的深度二次开发版本。在保留原版优秀的 HTML5/JS 框架基础上，我进行了全方位的内容革新，将其从一个简短的初作进化为一个拥有多分支、新剧情的沉浸式体验版本。

**🎮 在线游玩：** [点击这里开始你的冒险](https://aiwongs.github.io/the-house-game/)

---

## ✨ aiwongs 版核心改进 (3 Years Ago Updates)
相对于原版，本项目在以下维度进行了深度定制：

### 1. 深度内容重构、视觉美术重绘 (Graphics & UI)
* **全界面汉化**：对游戏内的文本、对话、道具说明及 UI 进行了精准的中文化处理，确保剧情表达自然。
* **UI 交互优化**：更新了 `menu.png` 菜单界面及部分场景贴图（如 `room.jpg`、`room_picture_snow.png`），使其更符合重制版的艺术风格。
* **剧情重写**：巧妙地改变了原有的故事走向，为游戏注入了全新的背景设定和叙事逻辑。
* **多分支路线**：新增了剧情分支，玩家的选择将引导至不同的结果，极大地提升了游戏的可玩性和探索欲。

### 2. 剧情与逻辑重构 (Story & Scripting)
* **脚本优化**：针对汉化后的文本框溢出、字体显示等细节问题进行了代码级修正。
* **多分支剧情设计**：通过对 `js/scenes.js` 和 `js/game.js` 的深度修改，重构了游戏的叙事走向，加入了全新的剧情分支和结局。
* **中文本地化**：对所有 HTML 页面（从 `intro.html` 到 `exit.html`）进行了完整的文本汉化与排版优化。
* **核心代码增强**：
    * 优化了 `js/audio.js`：支持更复杂的音频调度。
    * 修改了 `js/items.js` 和 `js/npcs.js`：支持新剧情下的道具交互与角色反应。

### 3. 音效环境重编 (Soundscape)
* **全面替换音轨**：针对新剧情，更新了大量的 MP3 资源。
* **关键场景音效**：
    * 重新配置了 `aquarium.mp3`、`corridor.mp3`、`void.mp3` 等核心场景的背景氛围音。
    * 引入了 `scene_corridor_phone.mp3` 等关键剧情交互音效，增强沉浸感。

### 4. 技术架构（基于原版）
游戏依然采用前端技术栈构建，但针对我的定制化内容进行了逻辑调整：
* **js/audio.js** - 重新定义了全新的音效资源池。
* **js/scenes.js** - 存储了我重新设计的剧情分镜与转场逻辑。
* **js/dialogue_box.js** - 适配了中文显示效果。

---

## 🛠️ 技术架构说明

本项目利用现代 Web 技术栈实现，核心文件分布如下： **逻辑重映射** & **资源管理**
* **`/js/`**：游戏大脑。包含 aiwongs 修改后的 `game.js`（主逻辑）、`scenes.js`（剧情分镜）及 `settings.js`，确保 `js/data.js` 能够准确保存新剧情线下的玩家进度。。
* **`/css/`**：视觉样式。主要基于 Less 编写，包含 `styles.css` 的最终编译版本。
* **`/sound/`**：听觉灵魂。包含所有重制版的背景音乐与交互音效。
* **`/images/`**：场景素材。包含所有重绘的静态资源与动画序列帧。

---

## 🙏 致谢与声明 (Credits)

### 原始框架 (Original Engine)
* **原作者**：Artur Kot (Original Creator)
* **A* 算法**：Andrea Giammarchi
* **核心框架**：jQuery, SoundManager 2, Modernizr, jStorage, Spritely.

### 本版贡献、二次开发 (Remastered By)
* **汉化 & 剧情改编**：aiwongs
* **美术 & 音效重编**：aiwongs

---

## ⚖️ 开源许可 (Licenses)

* **代码部分 (Code)**: 遵循 [MIT License](LICENSE.md)。
* **艺术素材 (Artwork)**: 遵循 [Creative Commons Attribution 3.0 License](https://creativecommons.org/licenses/by/3.0/)。

---

**注意**：本重制版旨在展示 Web 游戏开发的无限可能，欢迎通过 Issue 提交你的游玩反馈或发现的隐藏结局！
