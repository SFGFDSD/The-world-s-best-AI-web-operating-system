<div align="center">

# 🖤 AI 生成的 Web OS

**两个单文件 HTML，两次 AI 对话，碾压你四年的工程。**

</div>

---

## ⚠️ 先说几句不好听的

前端圈有一种项目，我称之为**「框架堆砌型 Web OS」**。

它们的作者通常是这样的：

> *"我用 TypeScript + React 写了一个 Web 操作系统！模块化架构！npm 包体系！OOP 类继承！多层抽象继承链！事件驱动架构！还发了 npm 包！开发了四年！Star 几千！"*

听起来很牛对吧？

然后你打开一看——

**文件系统？localStorage。**

**5MB 的 localStorage。**

2026 年了，你在写一个「操作系统」，文件系统用的是 `localStorage` + JSON 序列化？你那个抽象基类的 `content` 字段，存的是一个 JSON 字符串？你那些为了省空间设计的缩写键名，是为了塞进 5MB 的 localStorage？

你知道 OPFS 存在吗？你知道 `navigator.storage.getDirectory()` 能给你一个**真实的文件系统**吗？你知道浏览器可以存 **GB 级**的数据吗？

### 让我们看看这种「四年工程」的含金量

| 能力 | 这类 Web OS 项目 | AI 单次生成 |
|------|-------------------|------------|
| 存储后端 | localStorage (5MB) | OPFS + IndexedDB (GB级) |
| 文件系统 | OOP 类继承模拟 | 真实文件系统 API |
| 架构 | TypeScript + React + npm 包 | 单文件 HTML，零依赖 |
| 容量上限 | 5MB | 数十 GB |
| 二进制文件 | ❌ JSON 字符串 | ✅ 真实 Blob 落盘 |
| 大文件支持 | ❌ | ✅ GB 级 |
| 文件元数据 | 几个简写字段 | path/name/type/size/mime/created/modified |
| 拖放导入 | ❌ | ✅ |
| ZIP 解压 | ❌ | ✅ 内置无依赖解析器 |
| 搜索 | ❌ | ✅ |
| 文件降级 | 无 | OPFS → IndexedDB 自动回退 |
| 跨标签同步 | ❌ | ✅ storage event |
| 草稿自动保存 | ❌ | ✅ |
| 窗口管理 | React 组件 | 原生 DOM |
| 代码量 | 数千行 + node_modules | 单文件，打开即用 |
| 部署方式 | npm install + build | 双击 HTML 文件 |
| 开发时间 | **4 年** | **1 次 AI 对话** |

> 四年。写了四年。用 TypeScript + React + npm 包 + OOP 继承体系 + 事件驱动架构 + localStorage JSON 序列化 + 缩写键名省空间。
>
> 写了四年，文件系统还是 5MB 的 localStorage。
>
> 你那一层又一层的抽象基类，那个精心设计的事件系统，那个发到 npm 上的共享包——
>
> **它们加在一起，存不下一张手机照片。**

这不是工程，这是行为艺术。

你用最重的框架，写了最弱的文件系统。你用最复杂的架构，实现了最可怜的 5MB 上限。你把 `content` 字段 JSON.stringify 进 localStorage 的时候，有没有想过浏览器在 2019 年就给了你 `navigator.storage.getDirectory()`？

**你的继承链再长，也继承不出一个真实的磁盘写入。**

**你的事件系统再优雅，也 emit 不出一个 GB 级的文件。**

**你的 npm 包发得再多，也包不住 5MB 这个数字的尴尬。**

所以问题来了——

> **既然你写了四年还不如 AI 一次生成的好，那你这四年到底在写什么？**

答案很简单：你在写架构。你在写类型。你在写抽象。你在写一层套一层的继承链。你在写共享包里的事件系统。你在写 npm 包的 `package.json`。

**但你没有在写文件系统。**

因为一个真正的文件系统，需要的是 OPFS，不是 localStorage。需要的是 `getFileHandle`，不是 `JSON.stringify`。需要的是真实落盘，不是内存里的对象树。

这些事情，AI 知道。你不知道。

---

## 🖥️ 下面是正片

两个 AI 模型，各一次对话，各一个单文件 HTML，各一个完整的 Web 操作系统。

没有 TypeScript，没有 React，没有 npm 包，没有 node_modules，没有 build 步骤，没有 OOP 继承链，没有 EventEmitter。

**只有 OPFS、IndexedDB、窗口管理器、文件管理器、编辑器、浏览器、媒体播放器、计算器、设置面板——全部在一个 HTML 文件里。**

打开即用。双击运行。部署即上线。

---

<table>
<tr>
<td width="50%" valign="top">

## 🌊 Monsoon OS

**GPT-5.5-xHigh · 单次生成**

*OPFS Persistent Desktop*

一个以深青色为主调的 Web 桌面系统，文件存储于 OPFS 真实文件系统，刷新不丢，断网不散。

### 核心

- **OPFS 真实文件系统** — `navigator.storage.getDirectory()`，GB 级容量，真实二进制落盘
- **零依赖** — 不含任何第三方库（仅 Tailwind CDN 用于样式）
- **单文件** — 一个 HTML，双击即用

### 应用

| 应用 | 名称 | 功能 |
|------|------|------|
| 📁 | Tide Files | OPFS 文件资源管理器 |
| ✏️ | Salt Editor | 文本与代码编辑器 |
| 🌐 | Reef Browser | iframe 网页浏览器，支持 `vfs:///` 协议读取 OPFS 文件 |
| 🎬 | Lowtide Media | 音视频与图片播放器 |
| 🧮 | Abacus | 计算器 |
| ⚙️ | Monsoon Settings | 壁纸更换与存储管理 |

### 特性

- ✅ 窗口拖拽 / 缩放 / 最小化 / 最大化 / 关闭
- ✅ 拖放文件导入（桌面 & 文件管理器）
- ✅ ZIP / TAR / GZ / TGZ 无依赖解压
- ✅ 文件导出（DownloadURL 拖出 + Export 按钮）
- ✅ 自定义壁纸（图片文件设为壁纸）
- ✅ 启动动画 + 开始菜单 + 桌面图标
- ✅ 文件类型智能识别与关联打开
- ✅ OPFS 不可用时自动降级提示

### 文件系统 API

```
fs.mkdir(path)          fs.writeFile(path, content)
fs.readFile(path, text) fs.delete(path)
fs.rename(path, name)   fs.move(src, dest)
fs.copy(src, dest)      fs.exists(path)
fs.listChildren(path)   fs.getNode(path)
```

</td>
<td width="50%" valign="top">

## 🌿 Meadow OS

**Claude Opus 4.7 · 单次生成**

*A Quiet Computer*

一个以苔藓绿与暖纸色为主调的 Web 桌面系统，田园牧歌美学，安静而完整。

### 核心

- **OPFS 真实文件系统** — 真实文件句柄，二进制读写，GB 级容量
- **零依赖** — 纯原生 Web API，无任何框架
- **单文件** — 一个 HTML，双击即用

### 应用

| 应用 | 名称 | 功能 |
|------|------|------|
| 📁 | Files | 文件资源管理器 |
| ✏️ | Editor | 文本编辑器，支持语法高亮 |
| 🖼️ | Image Viewer | 图片查看器，缩放平移 |
| 🎬 | Media Player | 音视频播放器 |
| 📄 | PDF Viewer | PDF 文档查看器 |
| 🌐 | Browser | 网页浏览器 |
| 🧮 | Calculator | 计算器 |
| ⚙️ | Settings | 外观与存储设置 |

### 特性

- ✅ 窗口拖拽 / 缩放 / 最小化 / 最大化 / 关闭
- ✅ 拖放文件导入（桌面 & 文件管理器）
- ✅ ZIP / TAR / GZ 无依赖解压
- ✅ 文件导出
- ✅ 自定义壁纸（含 SVG 手绘壁纸 + 自定义图片）
- ✅ 开始菜单 + 桌面图标 + 右键菜单
- ✅ 文件类型智能识别与关联打开
- ✅ CSV / TSV 表格预览
- ✅ localStorage 偏好持久化（壁纸、图标位置）

### 文件系统 API

```
fs.mkdir(path)          fs.writeFile(path, content)
fs.readFile(path)       fs.unlink(path)
fs.rename(path, name)   fs.copy(src, dest)
fs.copyTree(src, dest)  fs.exists(path)
fs.readdir(path)        fs.stat(path)
fs.basename(path)       fs.normalize(path)
fs.dirSize(path)        fs.search(query)
```

</td>
</tr>
</table>

---

## 📊 正面对比：AI 生成 vs 「四年工程」

| | 这类 Web OS | Monsoon OS | Meadow OS |
|---|---|---|---|
| **生成方式** | 人工开发 4 年 | AI 单次生成 | AI 单次生成 |
| **文件数** | 数百 + node_modules | **1** | **1** |
| **存储后端** | localStorage (5MB) | OPFS (GB级) | OPFS (GB级) |
| **二进制文件** | ❌ JSON 字符串 | ✅ 真实 Blob | ✅ 真实 Blob |
| **文件元数据** | 几个简写字段 | path/name/type/size/mime/created/modified | path/name/size/mtime/isDir |
| **拖放导入** | ❌ | ✅ | ✅ |
| **ZIP 解压** | ❌ | ✅ | ✅ |
| **搜索** | ❌ | ✅ | ✅ |
| **PDF 查看** | ❌ | ❌ | ✅ |
| **图片查看器** | ⚠️ 缩略图 | ✅ | ✅ 缩放平移 |
| **文件降级** | 无 | ✅ | ✅ |
| **部署方式** | npm install + build | 双击 HTML | 双击 HTML |
| **依赖项** | React + npm 生态 | 零 | 零 |
| **代码可读性** | 分散在数百文件 | 单文件，一目了然 | 单文件，一目了然 |

---

## 🎯 所以，这意味着什么？

**不是 AI 要取代你，是你写的东西本来就不该存在。**

当你的「操作系统」文件系统上限是 5MB 的时候，你就不该叫它操作系统。当你的「虚拟文件」只是 localStorage 里的 JSON 字符串的时候，你就不该叫它文件系统。当你用四年时间堆出一个继承链，却连一个真实的磁盘写入都做不到的时候——

**你不是在做工程，你是在做表演。**

AI 不需要你的 OOP 继承链。AI 不需要你的事件驱动架构。AI 不需要你的 npm 包。AI 不需要你的 TypeScript 类型系统。

AI 只需要知道一件事：**浏览器给了你 OPFS，用它。**

就这么简单。四年没想明白的事，AI 一次对话就想明白了。

> **写了这么多年，不如让 AI 帮你搞一个文件系统。比你写的强多了。**
>
> **你自己写的那玩意儿，说好听点叫「虚拟文件系统」，说难听点——**
>
> **就是一坨 localStorage 里的 JSON。**

---

<div align="center">

*两个 AI，两次对话，两个完整的 Web 操作系统。*

*没有框架，没有依赖，没有构建步骤。*

*只有 OPFS 和一个 HTML 文件。*

**这就是 2026 年的软件开发。**

</div>
