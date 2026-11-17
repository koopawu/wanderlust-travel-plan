# Wanderlust Travel Plan

> 人生旅行清单：12 个梦想目的地，5 年出行时间线与预算规划。

一个深色杂志风格的单页旅行计划网站，涵盖目的地介绍、分项预算、最佳出行月份、签证提示、五年时间线和预算对比。

## 在线预览

启用 GitHub Pages 后访问：

**https://koopawu.github.io/wanderlust-travel-plan/**

## 主要特性

- 12 个梦想主题、13 段行程与完整预算明细（日本樱花季与花火大会分开规划）
- 按年份组织的 5 年旅行时间线
- 预算横向对比与年度汇总
- 滚动动效与响应式布局
- 图片地址集中管理，便于维护与替换
- 纯静态站点，无需安装依赖或执行构建

## 本地预览

在仓库根目录启动本地静态服务器：

```bash
python3 -m http.server 8080
```

然后访问 `http://localhost:8080`。

## 部署到 GitHub Pages

1. 打开仓库的 **Settings → Pages**。
2. 在 **Build and deployment** 中选择 **Deploy from a branch**。
3. Branch 选择 **main**，目录选择 **/(root)**，点击 **Save**。
4. 等待部署完成后，访问上方的在线预览地址。

## 项目结构

```text
wanderlust-travel-plan/
├── assets/
│   └── travel-images.js  # 目的地与背景图片地址
├── index.html            # 页面结构、样式与交互
├── .nojekyll             # 禁止 GitHub Pages 执行 Jekyll 处理
├── .gitignore            # 忽略系统与编辑器临时文件
└── README.md             # 项目说明
```

## 技术说明

- HTML / CSS / JavaScript
- React 18（CDN）
- Tailwind CSS（CDN）
- Babel Standalone
- 集中式图片资源配置

页面需要联网加载 CDN 脚本、字体和在线图片。目的地与背景图片地址统一维护在 `assets/travel-images.js`，替换图片时无需修改页面组件。

> 页面中的预算为基于中档消费、单人出行的估算范围，实际费用会因出发城市、汇率、预订时间与住宿选择而变化。签证政策请在出行前以官方最新要求为准。
