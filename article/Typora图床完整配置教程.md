## Typora + PicList + Gitee 图床完整配置教程

如果你经常写 Markdown 文档，那么 **Typora** 是一款非常好用的编辑器。而在图片管理方面，推荐搭配免费的图床工具 **PicList**，它支持一键上传图片到各类图床。我自己的方案是：**Typora + PicList + Gitee**，写作体验非常流畅。

## Typora设置

打开 **Typora**，依次进入 `文件 → 偏好设置 → 图像`，在上传服务中选择 **PicList**。
 不过因为我们还没有安装 PicList，所以接下来需要先安装软件。

![](https://gitee.com/da-qiang-classmate/typora/raw/master/image/image-20250823223254969.webp)

## 安装PicList

有两种方式可以安装：

1.**命令行安装**（推荐）

```
winget install Kuingsmile.PicList
```

**2. 安装包安装**

 下载安装包后直接运行即可：[点此下载](https://pan.xunlei.com/s/VOYWTpfZSMG5PFyL455ke_50A1?pwd=s7j6#)

## 安装插件

PicList 默认没有内置 Gitee 图床，所以需要单独安装插件。打开 PicList，点击左侧 **插件，搜索 `gitee` 并安装。

![](https://gitee.com/da-qiang-classmate/typora/raw/master/image/image-20250823222935347.webp)

## 图床设置

为了让界面更简洁，建议把用不到的图床隐藏，只保留 Gitee。

操作方法：
进入 **设置 → 上传**，往下找到 **“请选择显示在菜单的图床”**，取消勾选不需要的选项，只留下 Gitee。

![](https://gitee.com/da-qiang-classmate/typora/raw/master/image/image-20250825203516467.webp)

然后，点击 **图床 → gitee → 配置**，会看到以下参数需要填写：

- **配置名**：随便起个名字，方便区分
- **repo**：仓库名（如 `用户名/仓库名`）
- **branch**：`master` 或主分支名
- **token**：Gitee 生成的私人令牌
- **path**：存放图片的目录（例如 `image`）
- **customPath**：可选，自定义路径规则

![](https://gitee.com/da-qiang-classmate/typora/raw/master/image/image-20250825203600014.webp)

## 参数获取

1. 打开 [Gitee 官网](https://gitee.com/) 注册并登录账号，点击右上角 **+号 → 新建仓库**，勾选 “设置模板” 与 “选择分支模型”

![](https://gitee.com/da-qiang-classmate/typora/raw/master/image/20250825220835730.webp)

2. 之后点击个人头像，点设置-私人令牌，生成新令牌

![](https://gitee.com/da-qiang-classmate/typora/raw/master/image/rerz.webp)

这样，Typora + PicList + Gitee 的图床方案就配置好了，之后写 Markdown 时插入的图片会自动上传到 Gitee，并返回在线链接，非常省心。












