# TCompress
###  Hello,这是一个Android图片压缩库
  压缩方面：尺寸、采样、质量三个方面进行压缩</br>
  优化：三星等部分手机的图片角度处理</br>
  扩展：压缩后图片最大宽高设定（压缩后尺寸接近设定最大值）、质量、格式、配置设定</br>
###  预览图:<br>
  <img width="350"  src="https://github.com/HoldMyOwn/TCompress/blob/master/preview/a.jpg"/><br>
###  创建对象:
<pre>
  //可以构造者方式设置,也可以创建对象设置属性值(不设定采用默认配置)
        Compress compress = new Compress.Builder()
                .setMaxWidth(700)
                .setMaxHeight(900)
                .setQuality(80)
                .setFormat(Bitmap.CompressFormat.JPEG)
                .setConfig(Bitmap.Config.RGB_565)
                .build();
//        Compress compress = new Compress();
//        compress.setConfig(Bitmap.Config.RGB_565);
//        compress.setFormat(Bitmap.CompressFormat.WEBP);
//        compress.setQuality(80);
//        compress.setMaxWidth(800);
//        compress.setMaxHeight(800);
</pre>
###  压缩图片:
<pre>
     //支持四种压缩转化，文件、Bitmap到压缩后的文件、Bitmap
        File compressedFile = compress.compressedToFile(mFile);
        //另外三种
//        File compressedFile1 = compress.compressedToFile(mBitmap);
//        Bitmap compressedBitmap = compress.compressedToBitmap(mFile);
//        Bitmap compressedBitmap1 = compress.compressedToBitmap(mBitmap);
</pre> 
###   具体细节用法,下载查看Demo
###   模板依赖:&nbsp;&nbsp;项目里面的TCompress模板
###   gradle依赖:&nbsp;&nbsp;&nbsp;compile&nbsp;'com.jkt:tcompress:1.0.0'


