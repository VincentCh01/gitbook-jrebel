# gitbook 安装

---

### gitbook 安装

* 下载安装node.js

  我们需要依赖node.js的npm安装包来安装gitbook。  
  [node.js 8.12.0 TLS](https://nodejs.org/dist/v8.12.0/node-v8.12.0-x64.msi "点击下载")

* 检查配置

  ![image](https://note-1255877116.cos.ap-guangzhou.myqcloud.com/nodejs.png)  
node.js安装成功

  ![image](	https://note-1255877116.cos.ap-guangzhou.myqcloud.com/npm.png)  
  npm安装成功

* 全局安装gitbook

  ```
  npm install gitbook-cli -g
  ```

  ![image](https://note-1255877116.cos.ap-guangzhou.myqcloud.com/gitbook.png)
  gitbook 安装成功

  在一个有markdown文件的目录下可执行命令，启动gitbook服务,默认端口号 4000
  ```
  gitbook serve
  ```
  ![image](https://note-1255877116.cos.ap-guangzhou.myqcloud.com/gitbook-sample.png)
  ![image](/asserts/456.png)

* gitbook 输出 pdf格式

  ```
  gitbook pdf
  ```
  ![pdf](/asserts/789.png)  
  ps: 此处需要下载[gitbook-pdf](https://calibre-ebook.com/download)依赖  
  ![gitbook-pdf](/asserts/222.png)
