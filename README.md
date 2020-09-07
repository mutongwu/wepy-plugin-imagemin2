# wepy 图片压缩插件

# 功能与wepy-plugin-imagemin一致，只是升级了依赖的压缩库 imagemin 及其 插件的版本
# 注意压缩插件的参数有变化

## 安装

```
npm install wepy-plugin-imagemin2 --save-dev
```

## 配置`wepy.config.js`

```
module.exports.plugins = {
    'imagemin2': {
        filter: /\.(jpg|png)$/,
        config: {
            'jpg': {
            	quality: 80
             },
            'png': {
                quality: [0.6, 0.8]
            }
        }
    }
};
```


## 参数说明

[imagemin](https://github.com/imagemin/imagemin)