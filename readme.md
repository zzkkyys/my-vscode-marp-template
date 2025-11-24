
## 1. 配置VSCode

使用vscode打开项目文件夹后，需要在`.vscode`文件夹下的`settings.json`中，添加themes文件路径：

```bash
{
    "markdown.marp.themes": [
        "./themes/blue.css",
        "./themes/xxxxxxx.css",
        "/Users/xxxx/yyy/xxx.css"
    ]
}
```

当然，如果themes是全局的话，那么可以把上述配置添加到VSCode中全局`settings.json`中。


## 2. 使用


在vscode中新建一个`md`文件，然后在md最上面的frontmatter中添加：
```text
---
marp: true
theme: blue
paginate: true
---
```
其中，各个参数分别表示：
1. `marp: true`：这是一个必需的指令，用于告诉 Marp for VS Code 插件，这个 Markdown 文件应该被当作一个 Marp 幻灯片来处理。
2. `theme: blue`：指定幻灯片使用的主题。在这里，它使用了名为 `blue` 的主题。这个主题可以是 Marp 内置的（如 `default`, `gaia`, `uncover`），也可以是我们在 `settings.json` 中定义的自定义主题。
3. `paginate: true`：启用页码。设置为 `true` 后，每张幻灯片的角落会自动显示页码。



除了以上参数，还有一些常用的指令：
- `size: 16:9`：设置幻灯片的尺寸比例，默认为 `16:9`。也可以设置为 `4:3`。
- `header: 'My Presentation'`：在每页幻灯片顶部添加页眉。
- `footer: '© 2025 My Company'`：在每页幻灯片底部添加页脚。

## 3. 幻灯片分页

在 Marp 中，使用 `---` (三个或更多的连字符) 来分隔每一页幻灯片。

```markdown
# 第一页

这是第一页的内容。

---

# 第二页

这是第二页的内容。
```

## 4. 导出幻灯片


![](https://ayyyyy.sbs/2025/11/94cd7d67bea2ba50a6f5dccca7ab1bbb.png)



编写完成后，可以点击 VSCode 右上角的 Marp 图标，然后选择“Export slide deck...”。Marp 支持导出为多种格式，包括：
- **HTML**
- **PDF**
- **PPTX** (PowerPoint)
- **PNG** (仅导出第一页)
- **JPEG** (仅导出第一页)

选择你需要的格式即可完成导出。