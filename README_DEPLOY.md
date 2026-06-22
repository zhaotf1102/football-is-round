# 足球是个圆的 v1.2 - 公网部署包

这是一个纯静态网页项目，核心文件是 `index.html`。

## 最快上线方式：Netlify Drop
1. 打开 Netlify 并登录。
2. 找到 Deploy / Add new site / Deploy manually / Drop folder 类似入口。
3. 上传整个 `football_is_round_v1_2_public_deploy` 文件夹。
4. 部署成功后会生成一个 `*.netlify.app` 公网链接。

## Vercel 方式
1. 新建 GitHub 仓库，把本文件夹里的所有文件上传进去。
2. 在 Vercel 里 New Project，导入该 GitHub 仓库。
3. Framework 选择 Other / Static；Build Command 留空或 `npm run build`；Output Directory 留空或 `.`。
4. 部署后会生成一个 `*.vercel.app` 公网链接。

## GitHub Pages 方式
1. 新建 GitHub 仓库，把本文件夹里的所有文件上传到仓库根目录。
2. Settings → Pages → Source 选择 Deploy from a branch。
3. Branch 选择 main / root。
4. 保存后等待 Pages 构建完成。

## 注意
- 当前版本是前端静态原型，浏览器端不能稳定抓取外部数据源；v1.3 建议加入 Python 后端爬虫/数据清洗服务。
- 模型使用前仍应登记可靠数据源，避免垃圾数据污染 EV 计算。
