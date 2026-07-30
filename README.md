# 深部煤层气井下数据诊断平台

探微知流团队 - 国创赛作品

## 部署说明

### 方法一：GitHub Pages（推荐）

1. 注册 GitHub 账号（https://github.com）
2. 点击右上角 "+" → New repository
3. 仓库名填 `cbm-platform`，选 Public，点 Create repository
4. 点击 "uploading an existing file" 链接
5. 把本文件夹内**所有文件和文件夹**拖进去（包括 .nojekyll 文件！）
6. 点 Commit changes
7. 进入仓库 Settings → 左侧 Pages → Source 选 `main` 分支 → 点 Save
8. 等待1-2分钟，访问 `https://你的用户名.github.io/cbm-platform/`

### 方法二：Vercel（更快）

1. 注册 https://vercel.com（可用 GitHub 登录）
2. 先用方法一把代码传到 GitHub
3. Vercel 中点 New Project → 导入仓库 → 直接 Deploy
4. 30秒后访问 `https://cbm-platform.vercel.app/`

## 文件结构

```
cbm-platform-deploy/
├── index.html              ← 主页面（原"诊断平台原型.html"）
├── .nojekyll               ← 必需！防止GitHub忽略_shared文件夹
├── README.md               ← 本说明文件
└── _shared/
    └── js/
        └── echarts.min.js  ← 图表库
```

## 注意事项

- `index.html` 必须叫这个名字，GitHub Pages 默认打开 index.html
- `.nojekyll` 文件必须有，否则 `_shared` 文件夹下划线开头会被 GitHub 忽略
- 上传时确保 `_shared/js/echarts.min.js` 的目录结构不变
