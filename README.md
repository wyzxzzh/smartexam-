# SmartExam - 智能出题系统

基于课本内容的初中练习题自动生成工具，利用 DeepSeek V3 大模型能力，根据教师输入的教材文本或知识点，自动生成标准化的初中练习题。

## 功能特点

- **智能出题**：根据教材内容自动生成单选题、填空题、简答题
- **多学科支持**：支持语文、数学、英语、科学、历史与社会等学科
- **难度分级**：提供基础 (C)、提升 (B)、培优 (A) 三个难度级别
- **自定义题量**：可自由设置各题型的数量
- **答案解析**：每道题都提供详细的答案解析
- **Word 导出**：支持导出格式完美的 Word 文档，数学公式正确显示
- **标准格式**：符合标准试卷格式，字体、字号、行间距规范

## 技术栈

- **前端框架**：Streamlit
- **AI 交互**：OpenAI Python SDK (连接 DeepSeek API)
- **文档转换**：pypandoc + python-docx
- **环境管理**：python-dotenv

## 安装步骤

### 1. 安装 Pandoc

访问 [Pandoc 官网](https://pandoc.org/installing.html) 下载并安装 Pandoc。

### 2. 安装 Python 依赖

```bash
pip install -r requirements.txt
```

### 3. 配置 API Key

在 `.streamlit/secrets.toml` 文件中配置 DeepSeek API Key：

```toml
deepseek_api_key = 'your_api_key_here'
```

## 运行应用

```bash
streamlit run app.py
```

## 使用说明

1. 在侧边栏设置学科、难度、题量等参数
2. 在主界面输入教材内容或知识点
3. 点击"生成练习题"按钮
4. 等待 AI 生成练习题
5. 下载 Word 或 Markdown 文档

## 版权信息

© 海盐县钟战华

## 许可证

MIT License
