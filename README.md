<h1 align="center">豆米 Domi 下载</h1>

<p align="center">
  面向投资研究与项目管理的 Mac 桌面智能工作台。
</p>

<p align="center">
  <a href="https://github.com/1DeepSheep/domi-releases/releases/latest"><strong>下载最新版</strong></a>
  ·
  <a href="https://github.com/1DeepSheep/domi-workbench">功能介绍与源码</a>
  ·
  <a href="https://github.com/1DeepSheep/domi-plugin">Domi 插件</a>
</p>

## 怎么安装

1. 打开右侧 [Releases](https://github.com/1DeepSheep/domi-releases/releases/latest)。
2. 下载名称以 `arm64.dmg` 结尾的文件。
3. 打开 DMG，把「豆米」拖入“应用程序”文件夹。
4. 启动豆米，按向导检查 Codex 登录、选择资料库，并决定是否连接 PLAUD。

公开安装包经过 Developer ID 签名和 Apple 公证。当前版本仅支持 Apple Silicon Mac。

## 安装前准备

豆米通过本机 Codex 执行任务。请先安装并登录 Codex：

```bash
codex --version
codex login status
```

尚未安装时请参考 [OpenAI Codex 官方文档](https://developers.openai.com/codex/)。

## 它能做什么

- 自动更新并筛选行业新闻；
- 研究公司、项目、创始人和投资机构；
- 生成会议纪要、投资快评、IC 材料和研究报告；
- 管理项目、人物、Markdown、图片与其他资料；
- 选择完全本地的 SQLite + Markdown，或连接自己的飞书 Base + Wiki；
- 按需连接 PLAUD；暂时不用时可以在首次设置中跳过。

豆米会自动安装配套 Domi 插件。用户数据、目录映射和连接设置保存在本机，更新应用不会清空。

完整说明、隐私设计和源码运行方法见 [domi-workbench README](https://github.com/1DeepSheep/domi-workbench#readme)。

## 校验下载文件

每个版本都附带 `SHA256SUMS.txt`。下载后可在终端校验：

```bash
shasum -a 256 -c SHA256SUMS.txt
```

`latest-mac.yml`、ZIP 和 blockmap 文件用于应用内自动更新；普通安装只需下载 DMG。
