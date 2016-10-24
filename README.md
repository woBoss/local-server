# local-server
## 安装node

1. 新建一个文件夹test
2. 在该文件下创建一个server.js
3. 在cmd 中 该文件x夹下 npm init 初始化
4. 'npm install express --save'安装所配置的文件
5. 配置server .js(所配置方法如下展示)
6. 'node server.js'启动服务器

## 配置server.js
```javascript
const express = require("express"),
      app = express();
app.use(express.static("./static"));
app.get("/",(req,res,next) => {
	res.end("666");
});
app.listen(10000,()=>{
	console.log("Server runs at port 10000");
});
