### mpx官网

[官网地址，请戳我](https://didi.github.io/mpx/)

### vscode高亮、提示

    首先在vscode安装vue插件，然后设置里搜索files.associations，打开settings.json将后缀mpx的文件指向vue：

        "files.associations": {
                "*.mpx": "vue"
        }

### 静态图片资源处理

> 可以在资源地址后面加上查询字符串?fallback禁止base64

### 分包处理

```javascript
    // src/app.mpx
    "pages": [ 
        "pages/index/index",
        "pages/cart/index",
        "pages/user/index"
    ],
    "packages":[
        "./pagesOther/index?root=pagesOther"
    ],
```
