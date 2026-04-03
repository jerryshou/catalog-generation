# 目录自动生成 (catalog-generation)

一个 Obsidian 插件，每次打开仓库时自动扫描所有文件夹和 Markdown 文件，生成或更新目录索引文件。

## 功能

- **自动扫描**：打开仓库时自动扫描所有文件夹和 Markdown 文件
- **目录结构**：以嵌套标题形式展示文件夹层级
- **文件链接**：自动生成指向原始文件的 Wiki 链接
- **标题提取**：从每个 Markdown 文件中提取标题（h1-h4）并生成链接
- **灵活配置**：
  - 可自定义目录文件路径
  - 支持排除指定文件夹
  - 可开关启动时自动生成

## 安装

1. 从 GitHub 下载最新版本
2. 将 `main.js`、`manifest.json`、`versions.json` 复制到 `.obsidian/plugins/catalog-generation/` 目录
3. 在 Obsidian 设置中启用插件

## 使用

1. 启用插件后，打开仓库时自动生成 `目录.md`
2. 可在设置中调整：
   - **目录文件路径**：相对于仓库根目录的路径（默认：`目录.md`）
   - **排除的文件夹**：扫描时跳过的文件夹，多个用英文逗号分隔（默认：`.obsidian,ext`）
   - **启动时自动生成**：打开仓库时自动生成/更新目录

## 目录格式示例

```markdown
## folder-name

  - **[[path/to/file|filename]]**
    - [[path/to/file#标题1|标题1]]
    - [[path/to/file#标题2|标题2]]

## another-folder

  ### subfolder

    - **[[path/another|another]]**

      - [[path/another#章节|章节]]
```

## 许可证

MIT
