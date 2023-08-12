## 在 Hexo 自定义页面中添加 ECharts 热力图

### 第一步：创建新的 Hexo 页面

1. 打开您的 Hexo 项目，可以使用代码编辑器或终端。

2. 运行以下命令创建一个新页面。将 `your-page-name` 替换为您想要的页面名称（例如 `heatmap`）：

   ```
   bashCopy code
   hexo new page your-page-name
   ```

3. 这将在 `source` 目录下创建一个名为heatmap的文件夹。

### 第二步：添加 HTML 和 JavaScript 代码

  将index.html文件复制到heatmap文件夹。

### 第三步：配置 Front Matter

1. 在heatmap文件夹创建一个名为 `heatmap.md` 的 Markdown 配置文件，用于配置自定义页面的标题、布局等信息：

   ```
   shellCopy code$ cd source/heatmap
   $ touch heatmap.md
   ```

2. 编辑自定义页面配置文件： 使用文本编辑器（如 VSCode、Sublime Text 等）打开 `heatmap.md` 文件，然后将以下内容粘贴到文件中并进行适当的编辑：

   ```
   ---
   title: 热力图
   layout: default
   ---
   
   
   <!-- 网页内容将由 index.html 文件嵌入 -->
   <iframe src="index.html" width="100%" height="800px" style="border: none;"></iframe>
   
   ```

3. 根据需要自定义页面内容。您可以根据需要修改标题、布局等文本。

4. 生成并部署博客： 在完成上述步骤后，使用以下命令生成并部署博客：

   ```
   rubyCopy code$ hexo generate
   $ hexo deploy
   ```

   这将生成包含您的自定义页面的静态网页文件，并将其部署到您配置的远程仓库。
   
5. 查看自定义页面： 在完成部署后，您可以在浏览器中访问您的博客，然后导航到 `http://your-domain/heatmap` 来查看您添加的自定义页面。 
   
   
  

   