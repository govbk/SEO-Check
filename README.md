# 🔍 SEO检查器-网页篡改检测工具 Pro

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/govbk/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey.svg)](README.md)
[![Electron](https://img.shields.io/badge/Electron-28.1.0-47848f.svg)](https://electronjs.org/)
[![Vue](https://img.shields.io/badge/Vue-3.4.0-4fc08d.svg)](https://vuejs.org/)

> 专业的SEO检测和篡改检测工具，支持多User-Agent检测、智能伪装识别和语义相似性分析

## ✨ 效果展示
- **主界面**
[![主界面](https://github.com/govbk/SEO-Check/blob/main/%E4%B8%BB%E7%95%8C%E9%9D%A2.png)](https://raw.githubusercontent.com/govbk/SEO-Check/refs/heads/main/%E4%B8%BB%E7%95%8C%E9%9D%A2.png)

- **检测结果**
[![检测结果](https://github.com/govbk/SEO-Check/blob/main/%E6%A3%80%E6%B5%8B%E7%BB%93%E6%9E%9C.png)](https://raw.githubusercontent.com/govbk/SEO-Check/refs/heads/main/%E6%A3%80%E6%B5%8B%E7%BB%93%E6%9E%9C.png)

- **检测详情**
[![检测详情](https://github.com/govbk/SEO-Check/blob/main/%E6%A3%80%E6%B5%8B%E8%AF%A6%E6%83%85.png)](https://raw.githubusercontent.com/govbk/SEO-Check/refs/heads/main/%E6%A3%80%E6%B5%8B%E8%AF%A6%E6%83%85.png)

- **关键词配置**
[![关键词](https://github.com/govbk/SEO-Check/blob/main/%E5%85%B3%E9%94%AE%E8%AF%8D.png)](https://raw.githubusercontent.com/govbk/SEO-Check/refs/heads/main/%E5%85%B3%E9%94%AE%E8%AF%8D.png)

- **篡改检测设置**
[![篡改设置](https://github.com/govbk/SEO-Check/blob/main/%E7%AF%A1%E6%94%B9%E8%AE%BE%E7%BD%AE.png)]([https://github.com/govbk/](https://raw.githubusercontent.com/govbk/SEO-Check/refs/heads/main/%E7%AF%A1%E6%94%B9%E8%AE%BE%E7%BD%AE.png))
## ✨ 主要特性

### 🚀 核心功能
- **多User-Agent检测**：同时使用桌面端、移动端、搜索引擎三种User-Agent进行检测
- **智能篡改识别**：基于5维分析算法，识别网站SEO伪装和内容篡改
- **语义相似性分析**：采用Jaccard算法对比不同终端的内容差异
- **高性能并发检测**：支持最高50个URL同时检测，可配置并发数
- **批量URL处理**：支持批量导入和检测，一键处理大量URL

### 🔧 检测引擎
- **Python HTTPX**：高性能HTTP客户端，支持HTTP/2和连接池
- **智能重试机制**：指数退避算法，自动处理网络异常
- **URL标准化**：自动生成多种URL变体（http/https、www/非www等）
- **字符编码检测**：智能识别网页编码，确保内容解析准确性
- **响应行为分析**：检测异常响应时间和状态码差异

### 📊 数据分析
- **5维篡改分析**：
  - SEO元素分析（标题、描述、关键词）
  - 内容结构分析（HTML标签、脚本数量）
  - 隐蔽技术检测（JavaScript重定向、CSS隐藏）
  - 内容质量评估（SEO评分、关键词密度）
  - 响应行为分析（状态码、响应时间）
- **自适应阈值**：根据页面复杂度动态调整检测灵敏度
- **置信度评分**：0-100%的可疑度评分，精确量化风险等级

### 🎨 用户界面
- **现代化设计**：基于Element Plus的精美UI界面
- **实时进度显示**：检测过程可视化，支持暂停/恢复/停止
- **详细结果展示**：分类显示检测结果，支持筛选和排序
- **响应式布局**：自适应不同屏幕尺寸，支持深色/浅色主题
- **无菜单栏设计**：专业软件外观，去除传统桌面应用菜单

## 🛠️ 技术栈

### 前端技术
- **Vue 3** - 渐进式JavaScript框架
- **TypeScript** - 类型安全的JavaScript超集
- **Element Plus** - 基于Vue 3的组件库
- **Pinia** - Vue的状态管理库
- **Vue Router** - Vue.js官方路由管理器

### 后端技术
- **Electron** - 跨平台桌面应用框架
- **Node.js** - JavaScript运行时环境
- **Python HTTPX** - 现代异步HTTP客户端
- **BeautifulSoup4** - HTML解析库

### 构建工具
- **Vite** - 极速的前端构建工具
- **Electron Builder** - 跨平台Electron应用打包工具
- **TypeScript Compiler** - TypeScript编译器

## 📦 安装与使用

### 系统要求
- **操作系统**：Windows 10/11 (x64)、macOS 10.14+、Linux (x64)
- **Python**：3.7+ (可选，程序会自动检测)
- **内存**：建议4GB以上
- **存储空间**：200MB可用空间

### 快速开始

#### 方式1：下载预编译程序
1. 从Releases下载最新版本
2. 解压并运行 `SEO检查器 Pro.exe`
3. 首次运行会自动检测Python环境

#### 方式2：从源码构建
```bash
# 克隆项目
git clone https://github.com/your-repo/seo-checker-electron.git
cd seo-checker-electron

# 安装依赖
npm install

# 开发模式运行
npm run dev

# 构建生产版本
npm run build

# 构建便携版exe
npm run build:portable

# 构建安装版exe
npm run build:installer
```

### Python环境配置
```bash
# 安装Python依赖
pip install httpx beautifulsoup4 lxml

# 或使用项目内置的requirements.txt
pip install -r python/requirements.txt
```

## 🎯 使用指南

### 基本检测流程

1. **启动程序**
   - 运行 `SEO检查器 Pro.exe`
   - 检查Python环境状态（绿色🐍表示正常）

2. **配置检测参数**
   - 进入设置页面配置Python路径
   - 调整并发数和检测阈值
   - 启用多User-Agent检测

3. **执行检测**
   - 输入单个URL或批量导入URL列表
   - 点击"开始检测"按钮
   - 实时查看检测进度和结果

4. **分析结果**
   - 查看检测详情和篡改分析
   - 对比不同User-Agent的内容差异
   - 导出结果为CSV或JSON格式

### 高级功能

#### 多User-Agent检测
```
桌面端   [🖥️]  → 标准桌面版网页内容
移动端   [📱]  → 移动优化版本内容  
搜索引擎 [🔍]  → 机器人可见内容
```

#### 篡改检测算法
- **语义相似性**：Jaccard系数计算内容相似度
- **HTML结构分析**：标签数量、脚本统计、链接分析
- **隐蔽技术检测**：识别JavaScript重定向、CSS隐藏
- **内容质量评估**：SEO元素完整性、关键词密度
- **响应行为分析**：状态码一致性、响应时间异常

### 配置选项

#### 检测设置
```json
{
  "timeout": 30,              // 请求超时时间(秒)
  "maxConcurrent": 10,        // 最大并发数
  "followRedirects": true,    // 跟随重定向
  "verifyTLS": false,         // TLS证书验证
  "maxRedirects": 5           // 最大重定向次数
}
```

#### 篡改检测
```json
{
  "enabled": true,            // 启用篡改检测
  "semanticThreshold": 0.8,   // 语义相似度阈值
  "lengthTolerance": 0.2,     // 内容长度容忍度
  "cloakingLevel": "medium"   // 隐蔽技术检测级别
}
```

## 📊 检测示例

### 检测结果解读

#### 正常网站示例
```
URL: https://example.com
┌─────────────┬──────────┬────────┬─────────────┐
│ User-Agent  │ 状态码    │ 长度   │ 响应时间     │
├─────────────┼──────────┼────────┼─────────────┤
│ 桌面端      │ 200      │ 45KB   │ 850ms       │
│ 移动端      │ 200      │ 42KB   │ 920ms       │
│ 搜索引擎    │ 200      │ 44KB   │ 780ms       │
└─────────────┴──────────┴────────┴─────────────┘
✅ 检测结果：正常 (置信度: 15%)
```

#### 疑似篡改网站示例
```
URL: https://suspicious-site.com
┌─────────────┬──────────┬────────┬─────────────┐
│ User-Agent  │ 状态码    │ 长度   │ 响应时间     │
├─────────────┼──────────┼────────┼─────────────┤
│ 桌面端      │ 200      │ 67KB   │ 1200ms      │
│ 移动端      │ 200      │ 71KB   │ 1350ms      │
│ 搜索引擎    │ 200      │ 12KB   │ 450ms       │
└─────────────┴──────────┴────────┴─────────────┘
🚨 检测结果：高度可疑 (置信度: 89%)

差异分析：
- 搜索引擎版本内容长度异常 (-82%)
- 标题内容不一致
- 检测到JavaScript重定向代码
- 响应时间差异显著
```

## 📈 性能优化

### 检测性能
- **并发检测**：支持1-50个并发线程
- **连接复用**：HTTP连接池减少建连开销
- **智能缓存**：避免重复检测相同URL
- **内存优化**：流式处理大批量URL

### 建议配置
```
小批量检测（<100 URLs）  → 并发数: 5-10
中等批量（100-500 URLs） → 并发数: 10-20  
大批量检测（>500 URLs）  → 并发数: 20-30
```

## 🔧 开发指南

### 项目结构
```
seo-checker-electron/
├── electron/              # Electron主进程代码
│   ├── main.ts            # 应用入口
│   ├── preload.ts         # 预加载脚本
│   └── http-handler.ts    # HTTP请求处理
├── src/                   # Vue前端代码
│   ├── components/        # 公共组件
│   ├── views/            # 页面组件
│   ├── stores/           # Pinia状态管理
│   └── assets/           # 静态资源
├── python/               # Python检测引擎
│   ├── httpx_client.py   # 主检测脚本
│   └── requirements.txt  # Python依赖
├── public/               # 公共资源
└── scripts/              # 构建脚本
```

### 开发环境搭建
```bash
# 1. 克隆项目
git clone <repository-url>
cd seo-checker-electron

# 2. 安装Node.js依赖
npm install

# 3. 安装Python依赖
pip install -r python/requirements.txt

# 4. 启动开发服务器
npm run dev

# 5. 构建项目
npm run build
```

### API接口

#### IPC通信接口
```typescript
// 主进程 → 渲染进程
interface ElectronAPI {
  runHttpx(url: string, options: HttpOptions): Promise<ScanResult>
  runBatchHttpx(urls: string[], options: HttpOptions): Promise<ScanResult[]>
  checkPythonEnvironment(pythonPath?: string): Promise<PythonStatus>
  writeFile(filePath: string, data: string): Promise<boolean>
  readFile(filePath: string): Promise<string>
  getSystemInfo(): Promise<SystemInfo>
}
```

#### 数据结构
```typescript
interface ScanResult {
  id: string
  url: string
  title: string
  description: string
  keywords: string
  status: number
  timestamp: string
  userAgent: string
  responseTime?: number
  contentLength?: number
  isTampered?: boolean
  tamperDetails?: TamperDetails
}

interface TamperDetails {
  desktopContent?: string
  mobileContent?: string
  botContent?: string
  differences?: string[]
  suspiciousActivities?: string[]
  confidenceScore?: number
  analysisDetails?: AnalysisDetails
}
```

## 🐛 故障排除

### 常见问题

#### Python环境问题
```
问题：❌ Python环境不可用
解决：
1. 安装Python 3.7+
2. 在设置中配置正确的Python路径
3. 安装必需的Python库：pip install httpx beautifulsoup4
```

#### 检测失败问题
```
问题：检测失败或超时
解决：
1. 检查网络连接
2. 增加超时时间设置
3. 降低并发数
4. 检查目标网站是否可访问
```

#### 性能问题
```
问题：检测速度慢
解决：
1. 适当增加并发数
2. 检查Python环境性能
3. 使用SSD存储
4. 关闭不必要的安全软件
```

### 日志查看
```bash
# 应用日志位置
Windows: %APPDATA%/seo-checker-electron/logs/
macOS: ~/Library/Logs/seo-checker-electron/
Linux: ~/.local/share/seo-checker-electron/logs/
```

## 📄 许可证

本项目采用 [MIT 许可证](LICENSE)。

## 🤝 贡献指南

我们欢迎社区贡献！请阅读 [CONTRIBUTING.md](CONTRIBUTING.md) 了解详细信息。

### 贡献流程
1. Fork 项目
2. 创建功能分支
3. 提交更改
4. 推送到分支
5. 创建Pull Request

## 📮 联系我们

- **项目主页**：[GitHub Repository](https://github.com/govbk/SEO-Check)
- **问题反馈**：[Issues](https://github.com/govbk/SEO-Check/issues)
- **功能建议**：[Discussions](https://github.com/govbk/SEO-Check/discussions)

## 🙏 致谢

感谢以下开源项目：
- [Electron](https://electronjs.org/) - 跨平台桌面应用框架
- [Vue.js](https://vuejs.org/) - 渐进式JavaScript框架
- [Element Plus](https://element-plus.org/) - Vue 3组件库
- [HTTPX](https://www.python-httpx.org/) - Python HTTP客户端
- [Vite](https://vitejs.dev/) - 前端构建工具

---

<div align="center">
  <p><strong>SEO检查器 Pro</strong> - 让SEO检测更加专业和高效</p>
  <p>Made with ❤️ by SEO检查器</p>
</div>
