# soulcard-privacy

心卡 SoulCard 的隐私政策与支持页静态站点。通过 GitHub Pages 部署。

## 页面

- `/` (`index.html`) — 落地页，链接到隐私政策和支持页
- `/privacy.html` — 隐私政策（提交给 App Store Connect 的 Privacy URL）
- `/support.html` — 帮助与支持（提交给 App Store Connect 的 Support URL）

## 本地预览

```bash
python3 -m http.server 8000
# 然后浏览器打开 http://localhost:8000
```

## 部署

仓库 push 到 GitHub 后：

1. Repo Settings → Pages → Source 选 `Deploy from a branch`
2. Branch 选 `main` / `(root)`
3. 几分钟后 `https://<owner>.github.io/soulcard-privacy/` 生效

## App Store Connect 填写

- **Privacy Policy URL**: `https://<owner>.github.io/soulcard-privacy/privacy.html`
- **Support URL**: `https://<owner>.github.io/soulcard-privacy/support.html`

## 修改原则

- 改隐私政策后顺手把 `privacy.html` 顶部的"更新日期"也改一下
- 任何描述 App 收集 / 上传数据的措辞变更，必须先保证 App 本体行为对得上 —— 二者不能不一致
