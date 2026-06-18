# self get money

面向中文市场小单的前端接单展示页，当前主打：

- 小企业官网改版
- H5活动页
- 报名 / 咨询表单页面
- AI客服话术配置

## 本地查看

直接用浏览器打开：

```bash
open index.html
```

也可以启动一个静态服务：

```bash
python3 -m http.server 8080
```

然后访问：

```text
http://localhost:8080
```

## 文件结构

```text
.
├── index.html
├── assets/
│   └── wechat-qr.jpg
└── docs/
    ├── case-playbook.md
    ├── client-scripts.md
    └── cases/
```

## 部署建议

优先顺序：

1. GitHub Pages：免费，适合先展示。
2. Netlify / Vercel：免费，部署简单。
3. 国内服务器 / 宝塔：访问更稳定，但需要域名、备案和服务器成本。

当前是纯静态页面，不需要后端、不需要数据库、不需要构建工具。

详细部署清单见 `docs/deploy-checklist.md`。
