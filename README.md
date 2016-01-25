# NW.js_test
NW.js test
nwjs的bg-script 是无法access gui window的, 然而对于gui的新开窗口又是通过window的"new-win-policy"控制的 目前没找到合适的方法 在不修改网站源码的情况下, 限制对新窗口的打开, 能不能帮忙看下?

nwjs作者的回复: "你好，0.13.0测试版开始bg-script可以访问GUI window，可以试试看，如果是0.12版本可以在程序启动的时候先打开一个隐藏窗口，然后在里面调用nw.Window.open，然后就可以利用new-win-policy了。" 算是一种思路 
