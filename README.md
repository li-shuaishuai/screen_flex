# screen_flex
h5屏幕适配方案

index.html文件中js代码为未压缩代码   
index.min.html文件中js代码为压缩后代码     
注：请使用index.min.html文件中压缩后的代码

## 使用

1. 在头部添加meta标签`<meta name="viewport" content="width=device-width, initial-scale=1.0">`
   
2. 将index.min.html中的script标签代码拷贝放在头部

3. 使用时在css文件中`px`转`rem`：`css尺寸=设计稿标注尺寸/（设计稿横向分辨率/10）`     
   注：在less、scass等预编译语言中，可使用函数来进行`css`to`less`自动转换，也可使用sublime、vscode中的插件进行转换。

4. 字体大小设置举例：
   
   ```css
   li { 
     font-size: 12px
   }
   [data-dpr="2"] li {
    font-size: 24px
   }
   [data-dpr="3"] li {
    font-size: 36px
   }
   ```
   注：字体大小等请根据具体项目要求配置。

详细介绍请阅读：http://www.lishuaishuai.com/solution/614.html
