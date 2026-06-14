# TClaw 产品 Roadmap 2026 - 协同版

多人实时协同的产品 Roadmap 看板，基于 Firebase Realtime Database。

## 🚀 部署步骤（5分钟）

### Step 1: 创建 Firebase 项目（免费）

1. 打开 https://console.firebase.google.com/
2. 点击「添加项目」→ 输入项目名（如 `tclaw-roadmap`）→ 一路下一步
3. 进入项目后，左侧菜单选「Realtime Database」→「创建数据库」
4. 选 **测试模式**（允许所有读写，30天后可调整规则）
5. 点击项目设置（齿轮图标）→「常规」→ 往下滚到「您的应用」→ 点击 Web 图标（</>）
6. 输入应用昵称 → 注册 → 复制 `firebaseConfig` 对象

### Step 2: 填入配置

编辑 `index.html`，搜索 `FIREBASE_API_KEY`，把 Step 1 中的配置替换进去。

### Step 3: 部署到 GitHub Pages

1. 在 GitHub 创建新仓库（如 `tclaw-roadmap`）
2. 上传 `index.html` 到仓库
3. Settings → Pages → Source 选 `main` 分支 → Save
4. 等 1 分钟，访问 `https://你的用户名.github.io/tclaw-roadmap/`

### Step 4: 分享链接

把 GitHub Pages 链接发给团队，大家打开就能实时协同编辑！

## 📝 功能
- ✅ 实时同步：一人勾选，所有人立刻看到
- ✅ 添加事项：支持添加新的待办事项和分组
- ✅ 优先级标记：P0/P1/P2 三级优先级
- ✅ 进度统计：实时计算总进度百分比
- ✅ 导出 JSON：一键导出数据备份
- ✅ 恢复默认：重置为初始数据

## ⚠️ 安全说明
测试模式下数据库对公网开放。如需限制访问，可在 Firebase Console → Realtime Database → Rules 中设置规则。
