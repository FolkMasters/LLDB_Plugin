# lldb配置cat命令

1.下载libfooplugin.dylib文件（直接在当前页面上下载即可）

2.打开terminal.app(终端)

```
//将下载的文件移动到用户目录下
 🏡  /  mv ~/Downloads/libfooplugin.dylib ~/
 
//进入电脑根目录
 🏡  ~  cd /
 //创建并编辑.lldbinit文件
 🏡  /  vim .lldbinit
 
 //在打开的编辑页面上
 plugin load /Users/xxxxx/libfooplugin.dylib
```

3.重启一下xcode

4.运行代码，在断点处
![image](https://user-images.githubusercontent.com/9525575/156345351-55beb915-86dd-4ecc-869d-849c9e4eaea8.png)

获取到打印的地址通过  ‘cat address 0x000000010d7736a0’ 得到最终结果
![image](https://user-images.githubusercontent.com/9525575/156345560-18b648b9-89e6-4ee9-9e22-ab74396260ae.png)
