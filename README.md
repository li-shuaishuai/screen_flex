# screen_flex
h5屏幕适配方案

index.html文件中js代码为未压缩代码
index.min.html文件中js代码为压缩后代码

## 使用

1. 在头部添加meta标签`<meta name="viewport" content="width=device-width, initial-scale=1.0">`
   
2. 将index.min.html中的script标签代码拷贝放在头部

3. 使用时在css文件中`px`转`rem`：`css尺寸=设计稿标注尺寸/（设计稿横向分辨率/10）`

4. 字体大小设置：
   
   ```css
   li { 
     font-size: 24px
   }
   [data-dpr="3"] li {
    font-size: 36px
   }
   ```

详细介绍请阅读：http://www.lishuaishuai.com/solution/614.html
