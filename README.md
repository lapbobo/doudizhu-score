# 斗地主计分牌 🃏

简单好用的线下斗地主游戏计分工具，支持3位玩家自动计分。

## ✨ 特性

- 📱 **移动端优先** - 专为手机设计，操作简单流畅
- 💾 **自动保存** - 使用 localStorage 保存所有数据，刷新不丢失
- 🎨 **现代设计** - iOS Glassmorphism 风格，简洁美观
- ⚡ **数字滚动动画** - 分数变化时有流畅的动画效果
- 🔄 **历史记录** - 完整的游戏历史，支持撤销和删除
- 📊 **智能计算** - 自动计算分数，符合标准斗地主规则

## 🎮 如何使用

### 基本操作

1. **修改玩家名字**
   - 点击玩家的名字即可编辑
   - 编辑完成后点击空白处或按回车键保存

2. **开始记分**
   - 点击底部的 `+` 按钮
   - 在弹出的窗口中选择地主、叫分、炸弹数和胜负
   - 点击"确定"即可添加记录

3. **删除记录**
   - 点击历史记录右侧的 🗑️ 图标
   - 确认删除后分数会自动更新

### 计分规则

- **基础分** = 叫分 (1, 2, 3)
- **倍率**:
  - 0 炸弹 = x1
  - 1 炸弹 = x2
  - 2 炸弹 = x4
  - 3 炸弹 = x8
  - 4+ 炸弹 = x16

- **地主胜**:
  - 地主得分 = 基础分 × 2 × 倍率
  - 农民得分 = -基础分 × 倍率

- **农民胜**:
  - 地主得分 = -基础分 × 2 × 倍率
  - 农民得分 = 基础分 × 倍率

## 🚀 部署到 GitHub Pages

### 方法一：通过 GitHub 网页界面部署

1. 创建新仓库 `doudizhu-score`
2. 上传 `index.html` 文件
3. 进入仓库 Settings → Pages
4. 在 Source 中选择 `main` 分支
5. 点击 Save，等待几分钟后即可访问

### 方法二：通过命令行部署

```bash
# 初始化仓库
git init
git add index.html
git commit -m "Initial commit"

# 创建远程仓库并推送（需要先在 GitHub 上创建空仓库）
git branch -M main
git remote add origin https://github.com/你的用户名/doudizhu-score.git
git push -u origin main

# 启用 GitHub Pages
# 进入仓库 Settings → Pages → Source: main branch → Save
```

部署完成后，你的网站将可以通过 `https://你的用户名.github.io/doudizhu-score/` 访问。

## 📱 兼容性

- ✅ iOS Safari
- ✅ Chrome Mobile
- ✅ Android 浏览器
- ✅ 微信内置浏览器
- ✅ 支付宝内置浏览器

## 🛠️ 技术栈

- HTML5
- CSS3 (Flexbox, Grid, CSS Variables)
- Vanilla JavaScript (ES6+)
- localStorage API

## 📝 数据说明

所有数据都保存在浏览器的 localStorage 中，包括：
- 玩家名字和头像
- 当前分数
- 完整的历史记录

清除浏览器缓存会删除所有数据，请注意备份重要记录。

## 🎯 适用场景

- 朋友聚会
- 家庭娱乐
- 休闲游戏
- 任何需要斗地主计分的场合

## 📄 License

MIT License - 可自由使用和修改

---

享受游戏！🎉