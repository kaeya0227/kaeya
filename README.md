# Kaeya

经济学文献雷达网页。当前版本是可部署的静态网页原型，后续由 Codex 自动化或 GitHub Actions 更新文献数据。

## 当前包含

- `web/index.html`: 文献雷达网页
- `config/interests.json`: 研究兴趣、来源和期刊池配置
- `.github/workflows/pages.yml`: GitHub Pages 发布工作流

## 部署到 GitHub Pages

1. 把本文件夹内容上传到 `kaeya0227/kaeya` 仓库。
2. 打开 GitHub 仓库的 `Settings -> Pages`。
3. 在 `Build and deployment` 里把 `Source` 设为 `GitHub Actions`。
4. 打开 `Actions -> Deploy Pages`，手动运行一次，或等待下一次 push 自动运行。

发布后网页通常在：

```text
https://kaeya0227.github.io/kaeya/
```

## 自动更新路线

第一阶段建议使用 Codex 自动化生成文献卡片，然后更新这个仓库里的网页文件。这样可以保留 Codex 的总结能力，同时用 GitHub Pages 展示网页。

如果以后改为纯 GitHub Actions 云端抓取和总结，则需要配置模型 API Key。不要把 API Key 写进仓库文件，应放在 GitHub `Settings -> Secrets and variables -> Actions -> Secrets`。

## 版权提示

如果后续加入凯亚主题，请优先使用抽象冰元素、冰神之眼风格、深蓝银白色系和自制/授权图片。公开网页不要直接使用未授权角色立绘。
