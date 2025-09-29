# 小靈芽 AI 好友通訊錄 🤖💫

一個先進的 AI 好友管理和對話系統，採用現代化 Web 技術與 Supabase 後端架構。

## 🌟 項目特色

### 核心功能
- **AI 好友管理** - 個性化的 AI 角色管理系統
- **智能對話系統** - 基於 Claude API 的高質量對話體驗  
- **動態改名功能** - 用戶可自定義 AI 好友名稱，AI 會自動感知名稱變更
- **對話歷史管理** - 完整的聊天記錄保存與管理
- **響應式設計** - 完美適配桌面端和移動端設備

### 技術亮點
- **三段咒語系統** - 創新的動態提示詞工程架構
- **成長追蹤機制** - AI 角色隨對話次數動態成長
- **實時通訊** - 高效的前後端數據同步
- **現代化 UI** - 基於 Tailwind CSS 的漂亮界面

## 🚀 在線演示

**當前部署地址**: https://3vbkpuytcq60.space.minimax.io

## 🛠 技術架構

### 前端技術棧
- **React 18** - 現代化前端框架
- **TypeScript** - 類型安全的開發體驗
- **Vite** - 極速的構建工具
- **Tailwind CSS** - 實用優先的 CSS 框架
- **Radix UI** - 高品質的組件庫
- **React Router** - 客戶端路由管理

### 後端技術棧
- **Supabase** - 現代化 BaaS 平台
- **PostgreSQL** - 可靠的關係型數據庫
- **Deno Edge Functions** - 服務端邏輯處理
- **Row Level Security** - 數據安全保護

### 外部服務集成
- **Anthropic Claude API** - 高品質 AI 對話服務
- **Supabase Auth** - 用戶身份認證
- **Supabase Storage** - 文件存儲服務

## 📁 項目結構

```
xiaolingya-ai-contacts/
├── src/                        # 前端源代碼
│   ├── components/             # React 組件
│   ├── contexts/              # React Context
│   ├── hooks/                 # 自定義 Hooks
│   ├── lib/                   # 工具庫和配置
│   ├── App.tsx               # 主應用組件
│   └── main.tsx              # 應用入口
├── backend/                   # 後端代碼
│   └── supabase/
│       ├── functions/         # Edge Functions
│       └── tables/           # 數據庫表結構
├── docs/                     # 項目文檔
├── public/                   # 靜態資源
├── package.json             # 依賴管理
├── tsconfig.json           # TypeScript 配置
├── tailwind.config.js      # Tailwind 配置
└── vite.config.ts         # Vite 配置
```

## 🔧 核心功能實現

### 1. AI 好友管理系統
- 個性化頭像和基本信息
- 可自定義的 AI 性格設置
- 完整的好友資料頁面

### 2. 智能對話功能
- 基於 Claude API 的自然語言處理
- 支持上下文記憶的連續對話
- 實時消息發送和接收

### 3. 改名感知機制
- 用戶可實時修改 AI 好友名稱
- AI 自動感知名稱變更並在對話中體現
- 系統提示詞動態更新

### 4. 三段咒語系統 (開發中)
- **基底咒語**: 定義 AI 核心性格
- **成長咒語**: 基於對話階段的動態提示
- **記憶咒語**: 基於歷史互動的個性化提示

## 🚀 快速開始

### 環境要求
- Node.js 18+
- pnpm (推薦) 或 npm
- Supabase 項目

### 安裝步驟

1. **克隆項目**
```bash
git clone <repository-url>
cd xiaolingya-ai-contacts
```

2. **安裝依賴**
```bash
pnpm install
# 或者
npm install
```

3. **環境配置**
創建 `.env.local` 文件：
```env
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

4. **數據庫設置**
導入 `backend/supabase/tables/` 中的 SQL 文件到您的 Supabase 項目

5. **部署 Edge Functions**
```bash
supabase functions deploy
```

6. **啟動開發服務器**
```bash
pnpm dev
# 或者
npm run dev
```

## 🔧 部署指南

### 前端部署
```bash
pnpm build
pnpm preview
```

### 後端配置
1. 設置 Supabase 環境變量
2. 配置 Claude API 密鑰
3. 部署 Edge Functions
4. 設置數據庫 RLS 政策

## 📊 數據庫結構

### 核心表格
- `ai_friends` - AI 好友基本信息
- `conversations` - 對話會話管理
- `messages` - 消息記錄
- `user_profiles` - 用戶資料
- `growth_tracking` - 成長追蹤數據

## 🎯 功能路線圖

### 已完成 ✅
- [x] 基礎 AI 好友管理
- [x] 對話系統核心功能
- [x] 改名感知機制
- [x] 響應式 UI 設計
- [x] 用戶認證系統

### 開發中 🚧
- [ ] 三段咒語系統完整實現
- [ ] 多媒體消息支持
- [ ] 情感檢測功能

### 計劃中 📋
- [ ] 語音對話功能
- [ ] 圖片理解能力
- [ ] Mattermost 插件集成
- [ ] 移動端原生應用

## 🤝 貢獻指南

歡迎提交 Issue 和 Pull Request！

1. Fork 本項目
2. 創建功能分支 (`git checkout -b feature/amazing-feature`)
3. 提交更改 (`git commit -m 'Add amazing feature'`)
4. 推送分支 (`git push origin feature/amazing-feature`)
5. 創建 Pull Request

## 📝 許可證

本項目採用 MIT 許可證 - 查看 [LICENSE](LICENSE) 文件了解詳情

## 👥 作者

- **Waitin Chen** - 主要開發者

## 🙏 致謝

- Anthropic Claude API 提供強大的 AI 對話能力
- Supabase 提供優秀的 BaaS 服務
- 所有開源項目的貢獻者

---

## 📞 支持與反饋

如果您在使用過程中遇到問題或有改進建議，請：

1. 查看 [FAQ](docs/FAQ.md)
2. 提交 [Issue](issues)
3. 聯繫開發團隊

**讓我們一起構建更智能的 AI 對話體驗！** 🌟