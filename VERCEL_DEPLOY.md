---
AIGC:
    ContentProducer: Minimax Agent AI
    ContentPropagator: Minimax Agent AI
    Label: AIGC
    ProduceID: "00000000000000000000000000000000"
    PropagateID: "00000000000000000000000000000000"
    ReservedCode1: 304402203c813b713da5a5717d37cb04b0b19d7a9e951fe69ea603176daab8b1dd031f19022075df8a8cfe4c77300ac620554cb84cc038dc58f9985b33335489616419e83388
    ReservedCode2: 3045022100df4b0d4100aa213e9c57cdc97015ae7b1914dc0a31801e9c8b9b1c9d9e306be202206c1b96d1995643c408f6f2f29b0d216ac0fa8776786c50b87014067a100e823b
---

# Vercel 部署指南

## 方法一：使用 GitHub 部署（推荐）

### 步骤 1：上传代码到 GitHub
1. 登录 [GitHub](https://github.com)
2. 创建新仓库，命名为 `football-booking`
3. 将本地代码推送到 GitHub：
   ```bash
   cd /workspace/football-booking
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/你的用户名/football-booking.git
   git push -u origin main
   ```

### 步骤 2：连接 Vercel
1. 登录 [Vercel](https://vercel.com)
2. 点击 "New Project"
3. 导入你的 GitHub 仓库 `football-booking`
4. 配置保持默认，点击 "Deploy"

部署完成！Vercel 会自动构建并提供 URL。

---

## 方法二：使用 Vercel CLI 部署

### 步骤 1：安装 Vercel CLI
```bash
npm install -g vercel
```

### 步骤 2：登录 Vercel
```bash
vercel login
```

### 步骤 3：部署
```bash
cd /workspace/football-booking
vercel
```

按照提示操作：
- Set up and deploy? **Yes**
- Which scope? 选择你的用户名
- Want to modify settings? **No**

部署完成！

---

## 注意事项

1. **Supabase 配置已内置**：代码中已包含 Supabase 连接信息，部署后可直接使用
2. **实时同步**：Vercel 部署后同样支持实时同步功能
3. **自定义域名**：如需自定义域名，可在 Vercel 项目设置中添加

## 访问你的网站

部署成功后，Vercel 会提供一个类似以下格式的 URL：
- `https://football-booking.vercel.app`
- 或 `https://你的项目名.vercel.app`

你可以将这个 URL 分享给你的足球群成员！
