# cdn-blog

## 上传到GitHub仓库指令
    // 查看状态
	git status
	// 添加到库中
	git add .
	// 提交更新（引号内 为自定义信息说明）
	git commit -m '第一次提交'
	// 推送至远程仓库 
	git push
  ##  通过jsDeliver引用资源 ##
  ### npm ###
      // load any project hosted on npm (加载任何Github发布、提交或分支)
	https://cdn.jsdelivr.net/npm/package@version/file

	// load jQuery v3.2.1 （加载 jQuery v3.2.1）
	https://cdn.jsdelivr.net/npm/jquery@3.2.1/dist/jquery.min.js

	// use a version range instead of a specific version (使用版本范围而不是特定版本）
	https://cdn.jsdelivr.net/npm/jquery@3.2/dist/jquery.min.js
	https://cdn.jsdelivr.net/npm/jquery@3/dist/jquery.min.js

	// omit the version completely to get the latest one (完全省略该版本以获取最新版本）
	// you should NOT use this in production
	https://cdn.jsdelivr.net/npm/jquery/dist/jquery.min.js

	// add ".min" to any JS/CSS file to get a minified version (将“.min”添加到任何JS/CSS文件中以获取缩小版本，）
	// if one doesn't exist, we'll generate it for you (如果不存在，将为会自动生成）
	https://cdn.jsdelivr.net/npm/jquery@3.2.1/src/core.min.js

	// omit the file path to get the default file  (省略文件路径以获取默认文件）
	https://cdn.jsdelivr.net/npm/jquery@3.2

	// add / at the end to get a directory listing  (在末尾添加 / 以获取资源目录列表)
	https://cdn.jsdelivr.net/npm/jquery/
  ### GitHub使用 ###
  使用方法： 
 
    https://cdn.jsdelivr.net/gh/你的用户名/你的仓库名@发布的版本号/文件路径
	比如：
	//加载图片
	https://cdn.jsdelivr.net/gh/Zevs6/CDN/img/avatar.jpg

注意：版本号不是必需的，是为了区分新旧资源，如果不使用版本号，将会直接引用最新资源，除此之外还可以使用某个范围内的版本，查看所有资源等，具体使用方法如下：

    //加载任何GitHub版本，提交或分支
	//注意：我们建议对支持npm的项目使用npm
	https://cdn.jsdelivr.net/gh/user/repo@version/file
	//加载jQuery v3.2.1
	https://cdn.jsdelivr.net/gh/jquery/jquery@3.2.1/dist/jquery.min.js

	//使用版本范围而不是特定版本
	https://cdn.jsdelivr.net/gh/jquery/jquery@3.2/dist/jquery.min.js
	https://cdn.jsdelivr.net/gh/jquery/jquery@3/dist/jquery.min.js

	//完全省略该版本以获取最新版本
	//您不应该在生产中使用它
	https://cdn.jsdelivr.net/gh/jquery/jquery/dist/jquery.min.js

	//将“ .min”添加到任何JS / CSS文件以获取缩小版本如果不存在，我们会为您生成
	https://cdn.jsdelivr.net/gh/jquery/jquery@3.2.1/src/core.min.js

	//在末尾添加/以获取目录列表
	https://cdn.jsdelivr.net/gh/jquery/jquery/
