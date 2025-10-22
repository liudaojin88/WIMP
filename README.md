# 越南末端派送管理系统

## 项目简介

越南末端派送管理系统是一个专业的越南二段发运运单管理平台，提供完整的批次管理、订单跟踪、装箱装车和运输进度管理功能。

## 功能特性

### 🚚 核心功能
- **越南末端派送列表管理** - 完整的批次信息展示和管理
- **二段发运功能** - 支持订单勾选和批次创建/添加
- **运输批次编辑** - 详细的批次信息维护和状态跟踪
- **订单商品管理** - 支持批量添加、删除和编辑
- **装箱装车信息** - 完整的包装和运输信息管理
- **运输进度跟踪** - 实时进度展示和状态更新

### 📊 查询功能
- 支持14个查询维度，包括订单编号、父单号、第三方订单号等
- 智能筛选和模糊查询
- 批量操作和数据导出

### 🌐 技术特性
- 响应式设计，支持移动端访问
- 多币种金额显示（泰铢、美元、人民币）
- 越南语商品名称完整支持
- 现代化UI设计，用户体验优良

## 页面结构

```
├── index.html                    # 系统首页
├── vietnam-order-list.html       # 越南订单列表（含二段发运功能）
├── vietnam-delivery-list.html    # 越南末端派送列表
├── vietnam-batch-edit.html       # 运输批次编辑页面
└── README.md                     # 项目说明文档
```

## 快速开始

### 本地运行

1. **直接打开**
   ```bash
   # 直接用浏览器打开 index.html
   open index.html
   ```

2. **使用本地服务器**
   ```bash
   # 安装 serve（如果没有安装）
   npm install -g serve
   
   # 启动本地服务器
   serve -s . -l 3000
   
   # 访问 http://localhost:3000
   ```

### 云部署

#### 1. GitHub Pages 部署

```bash
# 1. 创建 GitHub 仓库
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/your-username/vietnam-delivery-management.git
git push -u origin main

# 2. 在 GitHub 仓库设置中启用 Pages
# Settings -> Pages -> Source: Deploy from a branch -> Branch: main
```

#### 2. Vercel 部署

```bash
# 1. 安装 Vercel CLI
npm install -g vercel

# 2. 部署到 Vercel
vercel

# 3. 按提示配置项目
```

#### 3. Netlify 部署

1. 将项目推送到 GitHub
2. 访问 [Netlify](https://netlify.com)
3. 选择 "New site from Git"
4. 连接 GitHub 仓库并部署

## 功能演示

### 二段发运流程

1. **选择订单**
   - 在越南订单列表页面勾选需要发运的订单
   - 点击"二段发运"按钮

2. **选择批次操作**
   - 添加到现有批次：将订单添加到已有的运输批次
   - 新建发货批次：创建新的运输批次

3. **填写批次信息**
   - 运输方式、承运商信息
   - 计划发货时间和送达时间
   - 系统自动验证订单兼容性

4. **批次管理**
   - 在末端派送列表查看和管理批次
   - 编辑批次详细信息
   - 跟踪运输进度

### 主要页面功能

#### 越南订单列表 (`vietnam-order-list.html`)
- 订单查询和筛选
- 批量选择和二段发运
- 订单状态管理
- 数据导出功能

#### 越南末端派送列表 (`vietnam-delivery-list.html`)
- 批次信息展示
- 展开/收起订单详情
- 批量操作功能
- 状态跟踪和管理

#### 运输批次编辑 (`vietnam-batch-edit.html`)
- 批次基本信息编辑
- 订单商品管理
- 装箱装车信息维护
- 运输进度跟踪

## 技术栈

- **前端框架**: 原生 HTML5 + CSS3 + JavaScript
- **UI 框架**: Bootstrap 5.3.0
- **图标库**: Bootstrap Icons 1.10.0
- **响应式设计**: 支持桌面端和移动端
- **浏览器兼容**: 现代浏览器（Chrome, Firefox, Safari, Edge）

## 系统要求

- **浏览器**: 支持 ES6+ 的现代浏览器
- **分辨率**: 最小 1024x768，推荐 1920x1080
- **网络**: 需要互联网连接加载 CDN 资源

## 部署配置

### 环境变量
无需特殊环境变量配置，系统为纯静态网站。

### CDN 依赖
- Bootstrap 5.3.0 CSS/JS
- Bootstrap Icons 1.10.0

### 服务器配置
- 支持静态文件托管的任意服务器
- 推荐启用 GZIP 压缩
- 建议配置 HTTPS

## 开发指南

### 代码结构
```
项目根目录/
├── index.html              # 系统入口页面
├── vietnam-order-list.html # 订单列表页面
├── vietnam-delivery-list.html # 派送列表页面
├── vietnam-batch-edit.html # 批次编辑页面
├── package.json           # 项目配置文件
└── README.md             # 说明文档
```

### 样式规范
- 使用 Bootstrap 5 组件和工具类
- 自定义样式采用 CSS3 特性
- 响应式设计遵循移动优先原则

### JavaScript 规范
- 使用现代 JavaScript (ES6+)
- 模块化函数设计
- 事件驱动的交互逻辑

## 许可证

MIT License - 详见 [LICENSE](LICENSE) 文件

## 贡献指南

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 创建 Pull Request

## 支持与反馈

- 问题反馈: [GitHub Issues](https://github.com/your-username/vietnam-delivery-management/issues)
- 功能建议: [GitHub Discussions](https://github.com/your-username/vietnam-delivery-management/discussions)

## 更新日志

### v1.0.0 (2024-10-21)
- ✨ 初始版本发布
- 🚚 完整的越南末端派送管理功能
- 📱 响应式设计支持
- 🌐 多语言和多币种支持
- 🎨 现代化UI设计

---

**越南末端派送管理系统** - 让物流管理更简单高效！