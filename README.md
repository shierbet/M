# 妙妙工具说明书

仅供技术学习

## 施工中

有很多种思路，如下提供两种

## bunnyCDN（也许好像大概是寄了，但是思路没问题，你可以使用任意CDN实现目标，包括国内的CDN提供商）

直接给cwm套个CDN不就得了

https://bunny.net/

注册前谷歌搜索`临时邮箱生成器`/`临时谷歌邮箱生成器`，用他们提供的邮箱进行注册，有一些临时邮箱被ban了，换一个就行，推荐使用`临时谷歌邮箱生成器`

提供14天免费1TB，还有5刀的余额，够用很久了，在账户余额的页面填入如下优惠码就可以领取5刀：`BUNNYFIVER`

建立一个新zone，回源地址填写`https://app.happybooker.cn/`或者`https://app.hbooker.com/`，创建完成就能拿到那个CDN地址填入设置即可

> 注意，禁止以/结尾，`https://ciweimao.b-cdn.net/` 应在设置中写 `https://ciweimao.b-cdn.net`

## Vercel（最好开个新号）

1、[Fork这个仓库](https://github.com/KoronekoCorp/M/fork)

2、注册一个vercel账户 [vercel](https://vercel.com/)  

3、在设置里绑定你的github账户

![bind github account](./asset/224318.jpg)

5、为了配置你的vercel仓库，请按照如下操作

导入一个github仓库: Overview => Add New... => Project.

![import git repository](./asset/224748.jpg)

点击 "Continue with GitHub" 按钮.

![looking your own rep](./asset/225212.jpg)

导入你刚刚fork的GitHub仓库

![Click Deploy](./asset/225542.jpg)

部署进度条在底下显示，等待其完成

![Deploy success](./asset/225816.jpg)

如下图所示就是你镜像的地址了，拿去设置里填入就行了

> 注意，禁止以/结尾，`https://m-doia.vercel.app/` 应在设置中写 `https://m-doia.vercel.app`

![Vercel Domain](./asset/230030.jpg)

### 更多设置，修改请求地区

如果你发现你的代理IP寄了，就需要修改你代理的执行地区，

> settings -> functions -> Function Region

![image](https://github.com/user-attachments/assets/bf95bd54-2d09-408e-aa5f-ed3490cfc171)

修改完成之后可能需要重新部署一次，我也不确定，好像没怎么用了，点击图中的redeploy

![image](https://github.com/user-attachments/assets/85af615b-2185-4fe6-8352-0ab3c0fe8b6d)

### 更多东西，你可以在部署完成之后把你的仓库直接删了，防止你的代理服务被公开，代理服务不会被一同删除
