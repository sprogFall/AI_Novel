# AI Novel Writer (AI小说家)

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

- **Backend**: Python with Flask framework
- **Frontend**: HTML5, TailwindCSS, Chart.js
- **AI Integration**: Compatible with vLLM API endpoints
- **Storage**: Local file system organization

### Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install python-docx beautifulsoup4 flask requests
   ```
3. Configure the LLM API endpoint in `main.py`:
   ```python
   VLLM_SERVER_HOST = "your_server_host"
   VLLM_SERVER_PORT = "your_server_port"
   ```

### Usage

1. Run the application:
   ```bash
   python main.py
   ```
2. Access the web interface at `http://localhost:5000`
3. Create a new project by providing:
   - Topic/subject
   - Content type (novel or course)
   - Structure parameters (chapters, sections, etc.)
4. Generate outline and confirm
5. Monitor generation progress in the task queue
6. Preview and download completed content

### Project Structure

```
├── main.py                 # Main application file
├── works_library/          # Generated content storage
│   ├── course/             # Course content
│   └── novel/              # Novel content
├── token_stats.json        # Token usage statistics
└── README.md              # This file
```

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

- **后端**：Python Flask框架
- **前端**：HTML5、TailwindCSS、Chart.js
- **AI集成**：兼容vLLM API端点
- **存储**：本地文件系统组织

### 安装说明

1. 克隆仓库
2. 安装依赖：
   ```bash
   pip install python-docx beautifulsoup4 flask requests
   ```
3. 在[main.py](file:///d:/GUOSHIYIN/models/ai%E5%B0%8F%E8%AF%B4%E5%AE%B6/main.py)中配置LLM API端点：
   ```python
   VLLM_SERVER_HOST = "your_server_host"
   VLLM_SERVER_PORT = "your_server_port"
   ```

### 使用方法

1. 运行应用：
   ```bash
   python main.py
   ```
2. 在浏览器中访问 `http://localhost:5000`
3. 通过提供以下信息创建新项目：
   - 主题/科目
   - 内容类型（小说或课程）
   - 结构参数（章节数、小节数等）
4. 生成大纲并确认
5. 在任务队列中监控生成进度
6. 预览和下载完成的内容

### 项目结构

```
├── main.py                 # 主应用文件
├── works_library/          # 生成内容存储
│   ├── course/             # 课程内容
│   └── novel/              # 小说内容
├── token_stats.json        # Token使用统计
└── README.md              # 本文件
```