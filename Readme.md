此项目旨在搭建一个IDA 插件模板，需要开发插件的时候git clone下来就可以使用，并且包含7.6版本的sdk，不需要重复配置环境。

因为IDA32和IDA64都是64位的，所以在选择x86/x64编译的时候一致选Release x64，但是需要额外做的是，

当你需要用ida32.exe的时候，也就是反编译32位的程序，需要在链接->常规->附加包含目录  改为x64_win_vc_32

链接器-常规-输出文件 改为你的IDA plugins的路径，方便测试

还有问题的话参考

https://blog.csdn.net/qq_34905587/article/details/108391159

https://ckcat.github.io/2020/12/02/IDA-%E6%8F%92%E4%BB%B6%E7%8E%AF%E5%A2%83%E9%85%8D%E7%BD%AE/




ida7.5及之后接口变了，在写插件的过程中会在sdk中添加一些必要的中文注释

