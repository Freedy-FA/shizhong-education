# 时中教育官网

公网地址：<https://freedy-fa.github.io/shizhong-education/>

## 目录结构

```
docs/            网站发布目录（GitHub Pages 只从这个目录或仓库根目录发布）
├── index.html   整站页面：内容、样式、脚本都在这一个文件里
└── logo.png     校徽（页面里 logo.png 缺失时会自动退回内置 SVG 版）
```

## 修改内容后怎么发布

```bash
git add -A
git commit -m "改了什么"
git push
```

推送后 1～2 分钟，线上自动更新。想看构建是否完成：

```bash
gh api repos/Freedy-FA/shizhong-education/pages/builds/latest -q .status
```

返回 `built` 即已生效。

## 待补充

- 页面底部的预约表单目前只弹一句提示，**没有收集数据**，需要接第三方表单服务或后端才能收到家长电话。
- 页脚的电话「400-800-1926」、地址「文化路 128 号」、ICP 备案号均为占位内容，上线推广前需替换为真实信息。
