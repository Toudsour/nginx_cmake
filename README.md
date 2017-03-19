##Nginx-CMake 

###简介
    这是一个用于生成Nginx对应CMakeList.txt的脚本
    主要在CLion对Nginx进行开发，调试时使用

###使用方法
- 1.将src中的cmake复制进nginx/auto里边
- 2.将nginx/configure中的`. auto/make`上加上`. auto/cmake`
- 3.正常编译Nginx(若没有指定目录,则相关文件在objs/下)
- 4.复制Nginx相关源码到你的项目中
- 5.用CLion创建项目,开始用CLion开发Nginx

TIPS:
- 推荐加上--builddir=<path>输出文件更方便
- Tengine有点麻烦，因为他强制需要openssl而且指定的库目录有点奇怪，所以还需要大家在本脚本的基础上多多修改


###最后
    哈哈哈，本人才疏学浅，这个脚本写的灰常low,若有dalao发现什么不好的地方，请多指教!
