# 自定义域名配置

## 需要先准备的内容

- 一个你已经买好的域名
- 域名的 DNS 管理权限
- GitHub 仓库 `percyymj/freelance-landing-page`

## GitHub Pages 绑定步骤

1. 打开仓库的 `Settings`。
2. 进入 `Pages`。
3. 在 `Custom domain` 填入你的域名。
4. 保存后等待 GitHub 校验。
5. 如果 GitHub 提示 DNS 未配置，就去域名服务商里补 DNS。
6. 等 HTTPS 生效后再正式对外使用。

## DNS 配置思路

如果你要绑定根域名，例如 `example.com`：

- 配置 `A` 记录指向 GitHub Pages 的地址
- 再补一个 `www` 的 `CNAME` 或者反向跳转

如果你要绑定子域名，例如 `www.example.com`：

- 配置一条 `CNAME` 指向 `percyymj.github.io`

## 仓库里需要的文件

如果最终使用自定义域名，仓库根目录通常需要一个 `CNAME` 文件，内容只有一行域名，例如：

```text
www.example.com
```

当前仓库还没有真实域名，所以先不要随便创建这个文件。

## 上线前确认

- 访问地址能打开首页
- `https` 正常
- 图片正常显示
- 刷新页面不报错
- 旧地址会自动跳转到新域名，或者至少清楚说明新地址

