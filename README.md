# Nexus Blog

Nexus Blog 是一个强大的 AI 驱动博客生成平台，结合了先进的大语言模型和现代前端技术，为用户提供智能化的内容创作体验。

## 📋 项目概览

Nexus Blog 旨在简化内容创作流程，通过 AI 技术帮助用户快速生成高质量的博客文章、小红书内容等，同时提供丰富的编辑和发布功能。

### 核心功能

- **AI 博客生成**：基于 LangGraph 工作流引擎，自动生成结构完整、内容丰富的博客文章
- **小红书内容创作**：专门针对小红书平台的内容格式，生成图文并茂的笔记
- **多种导出格式**：支持导出为 PDF、Word 等多种格式
- **定时任务管理**：通过 cron 表达式设置定时发布任务
- **智能图片生成**：根据内容自动生成相关图片
- **实时进度跟踪**：可视化展示内容生成过程
- **多风格支持**：提供学术、专业、幽默等多种写作风格

## 🛠️ 技术栈

### 后端
- **Python 3.10+**
- **Flask**：Web 框架
- **LangChain & LangGraph**：LLM 集成和工作流引擎
- **Jinja2**：模板引擎（用于 Prompt 管理）
- **Pydantic**：数据验证
- **多种工具库**：Pillow（图片处理）、python-docx（Word 导出）等

### 前端
- **Vue 3**：前端框架
- **Vite**：构建工具
- **Pinia**：状态管理
- **Vue Router**：路由管理
- **Tailwind CSS**：样式框架
- **TipTap**：富文本编辑器
- **Marked & Mermaid**：Markdown 渲染和图表支持
- **KaTeX**：数学公式渲染

## 📁 项目结构

```
nexus-blog/
├── api/                 # API 入口
│   └── index.py
├── backend/             # 后端代码
│   ├── infrastructure/  # 基础设施
│   │   └── prompts/     # Prompt 模板
│   ├── routes/          # API 路由
│   ├── services/        # 业务逻辑服务
│   ├── skills/          # 技能模块
│   ├── utils/           # 工具函数
│   ├── workflow_configs/ # 工作流配置
│   ├── config.py        # 配置文件
│   └── requirements.txt # Python 依赖
├── frontend/            # 前端代码
│   ├── src/             # 源代码
│   │   ├── components/  # Vue 组件
│   │   ├── composables/ # 组合式函数
│   │   ├── router/      # 路由配置
│   │   ├── services/    # API 服务
│   │   ├── stores/      # Pinia 状态管理
│   │   ├── views/       # 页面组件
│   │   └── App.vue      # 根组件
│   ├── package.json     # 前端依赖
│   └── vite.config.ts   # Vite 配置
└── README.md            # 项目说明
```

## 🚀 快速开始

### 环境要求

- **后端**：Python 3.10+
- **前端**：Node.js 16+

### 安装步骤

#### 1. 克隆项目

```bash
git clone https://github.com/jdw-art/nexus-blog.git
cd nexus-blog
```

#### 2. 安装后端依赖

```bash
cd backend
pip install -r requirements.txt
```

#### 3. 配置环境变量

复制 `.env.example` 文件为 `.env` 并填写相关配置：

```bash
cp .env.example .env
# 编辑 .env 文件，填写 API 密钥等配置
```

#### 4. 安装前端依赖

```bash
cd ../frontend
npm install
```

### 运行项目

#### 后端开发服务器

```bash
cd backend
flask run --host=0.0.0.0 --port=5000
```

#### 前端开发服务器

```bash
cd frontend
npm run dev
```

访问 `http://localhost:5173` 即可使用应用。

## 📖 使用指南

### 生成博客

1. 在首页输入博客主题和相关要求
2. 选择写作风格和其他高级选项
3. 点击「生成」按钮开始创作
4. 查看生成进度和结果
5. 编辑和完善内容
6. 导出或发布博客

### 小红书内容创作

1. 导航到「小红书创作」页面
2. 输入内容主题和要求
3. 选择图片风格
4. 生成图文内容
5. 预览和调整
6. 导出或发布

### 定时任务管理

1. 导航到「定时任务」页面
2. 创建新任务，设置执行时间和内容
3. 查看任务执行历史
4. 管理和编辑现有任务

## 🧪 测试

### 运行前端测试

```bash
cd frontend
npm test
```

### 运行后端测试

```bash
cd backend
python -m pytest
```

## 📚 文档

- **API 文档**：待补充
- **开发指南**：待补充
- **Prompt 模板**：`backend/infrastructure/prompts/` 目录

## 🔧 配置

### 后端配置

主要配置文件：`backend/config.py`

### 前端配置

主要配置文件：`frontend/src/stores/config.ts`

## 🤝 贡献

欢迎提交 Issue 和 Pull Request 来改进这个项目！

## 📄 许可证

[MIT License](LICENSE)

## 📞 联系方式

- 项目维护者：待补充
- 问题反馈：通过 GitHub Issues

---

**Nexus Blog** - 让内容创作更智能、更高效！