# iosapp
ipa installed by OTA
> OTA即Over-the-Air，是Apple在 iOS4 中新加的一项技术，目的是让开发者能够脱离Appstore，实现从自己的服务器下载并安装iOS应用。简单地说，就是用户只需要在Safari中点开一条链接，就能直接在主界面中安装App。
> ****
> OTA方式安装，是通过Safari解析链接中的**"itms-services://"**来实现的。
> `<a  href="itms-services://?action=download-manifest&url=https://raw.githubusercontent.com/JackWangCUMT/iosapp/master/manifest.plist">ipa download</a>`
>  OTA方式安装需要的文件：
>  
- .ipa  （http上就可以）
- .html （http上就可以，itms-services指向https下的plist文件）
- .plist（必须部署到**https**服务上，才能访问，指向http上的ipa文件）

----------
对于不能自己架设https服务器的童鞋，可以将plist文件托管到github上.
**Thanks GitHub**
