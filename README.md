# Mapbox 文档中文版

## 翻译进度

|模块|文件|翻译进度|说明|
|---:|----:|------:|-------:|
|API|all|0%|未开始|
|style-spec|all|0%|未开始|
|examples|all|0%|未开始|
|plugs|all|0%|未开始|

## 翻译需要依赖
1. nodejs 以大版本6.*为最佳;
2. jekyll
3. git 

## 项目目录说明
```
|-latest        最新版本的文档
    |- cn       最新版本文档的中文翻译
    |- en       最新版本文档的原版
|-v0.38.0       具体版本文档翻译(格式为 'v'+版本号)
    |-cn        版本文档的中文翻译
    |-en        文档的原版
|-index.html    首页文档
|-README.md     说明文档
```

## 获取翻译项目
```bash
$ git clone https://github.com/garyhan/mapbox-gl-js-cn
$ cd mapbox-gl-js-cn
```

## 开始说明
1. 如果不是当前版本的翻译请前往 mapbox-gl-js-cn/_config.yml中修改
```
baseurl: /mapbox-gl-doc-cn/v+[版本号]/cn
mapboxglbase: /mapbox-gl-doc-cn/v+[版本号]/cn/dist
```

2. 翻译API前往 mapbox-gl-js-cn/src下进行
    > 注意:请不要修改js文件名 以及@开头的参数

3. 翻译 style-spec 前往 mapbox-gl-js-cn/src/style-spec/reference/latest.js 中查找对应的json文件

4. 翻译 examples前往  mapbox-gl-js-cn/docs/_post/examples 下翻译每个文件即可

5. 翻译plugs 前往 mapbox-gl-js-cn/docs/_data/plugins.yml 中进行翻译文件

## 翻译
1. 打开要翻译的文件找到文件对应的 注释
2. 将注释替换为中文内容
3. 保存注释 
运行代码

```bash
$ npm run start-docs
```

运行完成后 浏览器中打开命令行中提示的路径
格式为: http://127.0.0.1:4000/mapbox-gl-js-cn/版本/