# 建筑施工安全题库 · 在线刷题

静态网页题库，可直接部署到 GitHub Pages，供本人及朋友在电脑或手机上访问。

## 目录结构

```text
.
├── index.html
├── questions.js
├── README.md
└── image/          # 将原「图片题」文件夹中的图片全部放入此处
    ├── 3253.jpg
    └── ...
```

题目数据中的图片路径已由 `图片题/文件名` 改为 `image/文件名`。上传时请把原文件夹改名为 `image`，不要修改图片文件名。

## 部署到 GitHub Pages

1. 在 GitHub 新建一个公开仓库（例如 `safety-quiz`）。
2. 将本目录全部文件上传到仓库根目录，务必包含 `image` 文件夹。
3. 打开仓库 **Settings → Pages**。
4. Source 选择 **Deploy from a branch**，Branch 选择 `main`（或 `master`），文件夹选择 `/ (root)`。
5. 保存后等待一两分钟，访问：

```text
https://<用户名>.github.io/<仓库名>/
```

若仓库名就是 `<用户名>.github.io`，则访问 `https://<用户名>.github.io/`。

## 本地预览

```bash
python3 -m http.server 8080
```

浏览器打开 `http://127.0.0.1:8080/`。

## 功能说明

- 顺序练习、随机练习、收藏重练
- 作答后显示正确答案与解析
- 错题本：自动收录、逐题练习、移出、清空、导出题号
- 电脑端与手机端自适应布局
- 作答记录保存在访问者自己的浏览器中，互不影响
