# 网页内容修改指南
本网站是由markdown文件提供内容，再由Jekyll进行静态渲染得到。如果需要对网页的外观样式进行修改，建议先通过以下链接快速学习一下Jekyll的基本工作原理，[Jekyll Document](https://www.jekyll.com.cn/docs/)。另一方面，如果只需要改动网页的内容，则找到相应的markdown文件进行修改即可。现提供简单指引如下：
### 修改初始页面
直接访问链接 `https://pku-tangent.github.io/` 或点击网站左上角的`PKU-TANGENT`都会默认进入网站初始界面。修改`_pages/about.md`即可改变网页内容。
### 修改 Publications
直接修改`_pages/publications.md`即可。
### 修改 Academic Activities
直接修改`_pages/academic_activities.md`即可。
### 修改 Research Grants
直接修改`_pages/research_grants.md`即可。
### 修改 Teaching
在`_teaching/`文件夹下新建一个md文件。具体内容可以参见已有的`Compiler.md`和`set&graph.md`等文件
### 修改 Students
在`_students/`文件夹下新建一个md文件。具体内容可以参见已有的`wenhao.md`和`liuyang.md`等文件。注意所有图片存在于`images/`文件夹下，每个人的默认头像是其中的`profile.png`，如需更改头像，则先上传图片到`images/`文件夹下，再将自己的md文件中的photo变量改成该图片的名字即可。
### 修改侧边栏图片及侧边栏其他信息
现在使用的侧边栏图片是`images/sujian.jpg`，要更换图片的话首先需要在`images/`文件夹下上传新图片，然后在`_config.yml`文件中将`sujian.jpg`（第84行，author下的avatar变量）改成新图片的名字。侧边栏的其它信息同样可以通过更改`_config.yml`文件中author下的其它变量来替换。
### 注意
提交更改后，一般要2~3分钟左右才能在网页上看到改动。如果想要有更强的交互性，可以尝试git clone该仓库然后进行本地调试。具体操作方式如下：
1. 确保已经安装了ruby-dev, bundler, and nodejs等工具：`sudo apt install ruby-dev ruby-bundler nodejs`。
2. 运行`bundle clean`来清理当前目录（不需要加`--force`选项）。
3. 运行`bundle install`来安装相关依赖。如果遇到error，尝试删除` Gemfile.lock`然后重试。
4. 运行`bundle exec jekyll serve`来生成HTML网页，在本地浏览器url栏输入`localhost:4000`访问页面。
5. 调试成功后再git push即可。