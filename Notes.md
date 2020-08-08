## 仓库选择

remi vs webmatic

## 常见问题

#### 安装yum install php72w-pecl-imagick报错

错误代码

```
Error: Package: php72w-pecl-imagick-3.4.3-1.2.w7.x86_64 (webtatic)
           Requires: libMagickWand.so.5()(64bit)
Error: Package: php72w-pecl-imagick-3.4.3-1.2.w7.x86_64 (webtatic)
           Requires: libMagickCore.so.5()(64bit)
```

运行 locate libMagickWand 命令查找原因
```
/usr/lib64/libMagickWand-6.Q16.so
/usr/lib64/libMagickWand-6.Q16.so.6
/usr/lib64/libMagickWand-6.Q16.so.6.0.0
```

初步分析可能是php72w-pecl-imagick依赖libMagickWand.so.5，而目前ImageMagick已经是libMagickWand-6
