## Smart Input 插件简介
对于母语为中文的开发者，写代码过程中经常需要在中/英输入法之间进行切换，而且由于不清楚当前处于哪种输入状态，有时输入到一半发现输入法错了，删除重新输入，有时切换了好几次都没有成功，实在太影响写代码了。

其实，在哪个位置需要使用哪种输入法是可以确定的，既然这样就可以让IDE帮助我们自动切换输入法。

JetBrains IntelliJ IDE可以通过Smart Input插件实现自动切换输入法，其核心功能是根据输入位置的上下文智能分析当前应该使用哪种输入法并自动切换，而且还可以通过光标的颜色来提醒当前是什么输入法。废话少说，先看效果。

## 注释场景
Java代码有三种注释方式，注释场景也是使用中文频率比较高的场景，下面动图演示了两种注释场景的效果。

![](https://mmbiz.qpic.cn/mmbiz_gif/CqgkJibaugibriceputbKwPlMl40icjWa4N9iaBLJIZLiahOSfCwmQv5LDbibqvJt7yEKtTptkhnialm6P2p6N3Y6VMmibg/640?wx_fmt=gif&wxfrom=5&wx_lazy=1)

识别到单行注释场景，自动切换为中文输入法。换行后编码，识别到光标位于编码区域，自动切换为英文输入法。整个过程无需主动切换输入法，写代码如丝般顺滑。光标红色表示当前使用中文输入法，灰色表示英文输入法。场景切换的时候会有浮层提示，熟悉后也可以关闭提示。

![](https://mmbiz.qpic.cn/mmbiz_gif/CqgkJibaugibriceputbKwPlMl40icjWa4N9ZPxMOqfCRQG685ib54q5MopQ8EtepAQ58rJHyda5MlVIBhpyXlDRuIA/640?wx_fmt=gif&wxfrom=5&wx_lazy=1)

对代码进行文档注释时，自动识别到当前处于文档注释场景，自动为您切换为中文输入法。中文输入法状态也可以进行简单的英文输入。

## Commit Message场景
一般我们都是使用中文写git的提交信息，该插件可以做到当Commit Message输入框获取到焦点时切换为中文输入法。

![](https://mmbiz.qpic.cn/mmbiz_gif/CqgkJibaugibriceputbKwPlMl40icjWa4N9u9nFB5yrrNc08oEDuHLtmZQ8WyuYJUqnicuz9E5s5dTnib9uj0x4Folw/640?wx_fmt=gif&wxfrom=5&wx_lazy=1)

## IdeaVim场景
习惯使用IdeaVim插件的人都知道在vim命令模式必须使用英文输入法，Smart Input插件可以在进入命令模式时自动切换为英文输入法。下图中光标为方块时表示进入了命令模式。

![](https://mmbiz.qpic.cn/mmbiz_gif/CqgkJibaugibriceputbKwPlMl40icjWa4N9hbLr38pVqvQicU9T0QnA8XRicffQr1fGsibFIrwicm5RvW5NOldd0VzASQ/640?wx_fmt=gif&wxfrom=5&wx_lazy=1)


完整文章请查看[微信公众号文章](https://mp.weixin.qq.com/s?__biz=MzIzMzcyNzA3Mw==&mid=2247483757&idx=1&sn=85260c90639afedc082ade647ca8a55b&chksm=e8807463dff7fd757e775066f4f07075d7c682b1d813f666bd3c195f471defdc659bb8466c29&scene=178&cur_album_id=2810769188716937217#rd)。关注微信公众号”开发效率“获取更多提升开发效率的方法。

![](https://smart-input-source-1315501506.cos.ap-shanghai.myqcloud.com/public/qrcode_for_weixingongzhong.jpg)

