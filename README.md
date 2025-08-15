# AI Novel Writer (AI小说家)

[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.0.0-orange.svg)](VERSION)

## English Version

### Project Overview

AI Novel Writer is an intelligent writing assistant that can automatically generate novels or course content based on user-provided topics. The system uses large language models to create detailed outlines, generate content with rich literary techniques, and maintain consistency throughout the story via a worldview system.

### Key Features

1. **Dual Content Generation Modes**:
   - Novel generation with rich literary techniques
   - Course content generation for educational materials

2. **Intelligent Worldview System**:
   - Automatically generates detailed world settings
   - Maintains consistency across chapters
   - Dynamically updates with story progression

3. **Advanced Task Management**:
   - Queue-based task processing
   - Breakpoint continuation support
   - Task cancellation capability

4. **Rich UI Interface**:
   - Modern web-based dashboard
   - Real-time log monitoring
   - Content preview and showcase mode
   - Token usage statistics

5. **Complete Content Management**:
   - Project library organization
   - ZIP archive download
   - Chapter-by-chapter content generation

### Technical Architecture

#### Backend Stack
- Python 3.x
- Flask Web Framework
- Requests library (for LLM API communication)
- python-docx (document processing)
- BeautifulSoup (content parsing)

#### Frontend Stack
- HTML5 + CSS3
- TailwindCSS (styling framework)
- Chart.js (data visualization)
- Marked.js (Markdown parsing)

#### AI Integration
- Compatible with vLLM API endpoints
- Support for custom model endpoints
- Token statistics and usage tracking

### Installation

#### System Requirements
- Python 3.7+
- pip package manager
- Accessible LLM API service (such as vLLM deployed models)

#### Installation Steps

1. Clone or download the project code
2. Install dependencies:
   ```bash
   pip install python-docx beautifulsoup4 flask requests
   ```

3. Configure LLM API connection parameters (in [main.py](file:///d:/GUOSHIYIN/models/ai%E5%B0%8F%E8%AF%B4%E5%AE%B6/main.py)):
   ```python
   VLLM_SERVER_HOST = "your_server_ip"     # Modify to your server IP
   VLLM_SERVER_PORT = "your_server_port"   # Modify to your server port
   SERVED_MODEL_IDENTIFIER = 'your_model_path'  # Modify to your model path
   ```

### Usage

#### Starting the Application
```bash
python main.py
```

After successful startup, the terminal will display:
```
==================================================
AI Content Factory v7.0 (Web UI) Started!
Please open your browser to http://127.0.0.1:5000
==================================================
```

#### Interface Function Description

1. **Create Project**:
   - Enter topic content
   - Select project type (novel/course)
   - Set structure parameters (number of chapters, word count, etc.)
   - Generate and confirm outline

2. **Project Library**:
   - View generated projects
   - Browse chapter content
   - Download ZIP archive

3. **Worldview**:
   - View novel worldview settings
   - Includes detailed information on characters, locations, rules, etc.

4. **Mind Library**:
   - View detailed planning for each chapter
   - Track generation status

5. **Task Queue**:
   - View current and historical tasks
   - Cancel running tasks

6. **AI Writing Showcase**:
   - Dynamic display of novel content
   - Typewriter effect playback

7. **Token Statistics**:
   - View API usage
   - Chart display of daily usage

### Project Structure

```
.
├── main.py                 # Main application file (contains all functions)
├── works_library/          # Generated content storage directory
│   ├── course/             # Course content directory
│   └── novel/              # Novel content directory
│       └── 《Work Title》/   # Specific work directory
│           ├── _worldview/ # Worldview settings
│           ├── _mind_library/ # Chapter planning (mind library)
│           └── Chapter files.md
├── token_stats.json        # Token usage statistics
├── README.md              # English README document
└── README_ZH.md           # Chinese README document
```

### Application Scenarios

- Online novel creation assistance
- Rapid course content generation
- Creative writing inspiration
- Batch production of educational resources
- Personal writing assistant tool

### Notes

1. Requires configuration of available LLM API service
2. Generation quality depends on the performance of the model used
3. Long-term operation is recommended to be deployed in a server environment
4. Generated content is for reference only, please pay attention to copyright issues when using

---

## 中文版本

### 项目概述

AI小说家是一个智能写作助手，能够根据用户提供的主题自动生成小说或课程内容。系统使用大语言模型创建详细的大纲，运用丰富的文学技巧生成内容，并通过世界观系统保持故事的一致性。

### 核心功能

1. **双重内容生成模式**：
   - 具有丰富文学技巧的小说生成
   - 教育材料的课程内容生成

2. **智能世界观系统**：
   - 自动生成详细的世界设定
   - 保持章节间的一致性
   - 随故事进展动态更新

3. **高级任务管理**：
   - 基于队列的任务处理
   - 支持断点续传
   - 任务取消功能

4. **丰富的UI界面**：
   - 现代化基于Web的仪表板
   - 实时日志监控
   - 内容预览和展示模式
   - Token使用统计

5. **完整的内容管理**：
   - 项目库组织
   - ZIP压缩包下载
   - 章节式内容生成

### 技术架构

#### 后端技术栈
- Python 3.x
- Flask Web框架
- Requests库（与LLM API通信）
- python-docx（文档处理）
- BeautifulSoup（内容解析）

#### 前端技术栈
- HTML5 + CSS3
- TailwindCSS（样式框架）
- Chart.js（数据可视化）
- Marked.js（Markdown解析）

#### AI集成
- 兼容vLLM API接口
- 支持自定义模型端点
- Token统计和用量跟踪

### 安装部署

#### 环境要求
- Python 3.7+
- pip包管理器
- 可访问的LLM API服务（如vLLM部署的模型）

#### 安装步骤

1. 克隆或下载项目代码
2. 安装依赖包：
   ```bash
   pip install python-docx beautifulsoup4 flask requests
   ```

3. 配置LLM API连接参数（在[main.py](file:///d:/GUOSHIYIN/models/ai%E5%B0%8F%E8%AF%B4%E5%AE%B6/main.py)文件中）：
   ```python
   VLLM_SERVER_HOST = "your_server_ip"     # 修改为你的服务器IP
   VLLM_SERVER_PORT = "your_server_port"   # 修改为你的服务器端口
   SERVED_MODEL_IDENTIFIER = 'your_model_path'  # 修改为你的模型路径
   ```

### 使用指南

#### 启动应用
```bash
python main.py
```

启动成功后，终端会显示：
```
==================================================
AI Content Factory v7.0 (Web UI) Started!
Please open your browser to http://127.0.0.1:5000
==================================================
```

#### 界面功能说明

1. **创建项目**：
   - 输入主题内容
   - 选择项目类型（小说/课程）
   - 设置结构参数（章节数、字数等）
   - 生成并确认大纲

2. **作品库**：
   - 查看已生成的项目
   - 浏览章节内容
   - 下载ZIP压缩包

3. **世界观**：
   - 查看小说的世界观设定
   - 包含人物、地点、规则等详细信息

4. **思维库**：
   - 查看各章节的详细规划
   - 跟踪生成状态

5. **任务队列**：
   - 查看当前和历史任务
   - 取消正在执行的任务

6. **AI写作秀场**：
   - 动态展示小说内容
   - 打字机效果播放

7. **Token统计**：
   - 查看API使用情况
   - 图表展示每日用量

### 项目结构

```
.
├── main.py                 # 主应用文件（包含所有功能）
├── works_library/          # 生成内容存储目录
│   ├── course/             # 课程内容目录
│   └── novel/              # 小说内容目录
│       └── 《作品名称》/     # 具体作品目录
│           ├── _worldview/ # 世界观设定
│           ├── _mind_library/ # 章节规划（思维库）
│           └── 各章节文件.md
├── token_stats.json        # Token使用统计
├── README.md              # 英文说明文档
└── README_ZH.md           # 本中文说明文档
```

### 应用场景

- 网络小说创作辅助
- 课程内容快速生成
- 创意写作灵感激发
- 教育资源批量制作
- 个人写作助手工具

### 注意事项

1. 需要配置可用的LLM API服务
2. 生成质量取决于所使用模型的性能
3. 长时间运行建议在服务器环境中部署
4. 生成的内容仅供参考，使用时请注意版权问题

## 💖 支持作者

如果你觉得这个项目对你有帮助，欢迎通过下方二维码赞赏支持作者的持续开发！

![赞赏码](dashang.png)

## ⚠️ 免责声明

本软件仅供学习和研究使用。使用者需要：

- 遵守相关法律法规
- 尊重知识产权
- 不得用于商业用途
- 对使用本软件产生的任何后果自行承担责任

⭐ 如果这个项目对你有帮助，请给个Star支持一下！ 💡 有商业化想法？欢迎交流合作，共同探索AI写作的无限可能！