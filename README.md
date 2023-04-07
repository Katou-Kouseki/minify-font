# 网页字体文件精简版

网页为了美观可能使用非系统字体，这时需要网页单独加载字体文件，字体文件一般比较大（接近 10M ），导致下载慢，并且字体文件中大部分字符都用不到。因此，通过删除不常用文字，来减小字体文件大小，加快网页速度。

### 使用资源

字体压缩工具

    https://ecomfe.github.io/fontmin/

3500 常用字数据

    https://github.com/DavidSheh/CommonChineseCharacter

| 字体（免费可商用） | 精简前 | 精简后 |                                                                                          |
| ------------------ | ------ | ------ | ---------------------------------------------------------------------------------------- |
| 思源黑体           | 8.1M   | 834K   | [下载](https://github.com/DeronW/minify-font/raw/master/dist/SourceHanSansCN-Medium.ttf) |
| 阿里巴巴普惠体     | 9.6M   | 1M     | [下载](https://github.com/DeronW/minify-font/raw/master/dist/Alibaba-PuHuiTi-Medium.ttf) |
| OPPO San           | 10.1M  | 1.1M   | [下载](https://github.com/DeronW/minify-font/raw/master/dist/OPPOSans-M.ttf)             |

### 手动精简方法

1. 拷贝字体文件到 fonts 目录
1. 修改 index.js 文件，把新字体文件添加到编译方法中
1. 执行 build 方法

```shell
npm i
npm run build
```

新的精简版字体文件输出到 `dist` 目录中.
