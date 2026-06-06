# ReadCoach AI

ReadCoach AI is Archer's customized open-source AI reading coach for foreign-language learning. It turns any topic into a guided reading lesson with level-aware articles, translations, vocabulary help, grammar analysis, sentence rewrites, and comprehension quizzes.

ReadCoach AI 是 Archer 维护的开源 AI 外语阅读教练项目。它可以把任意主题生成适合学习者水平的阅读材料，并提供译文、词汇释义、语法分析、句子改写和理解测验。

Repository: [github.com/Archer-hx/ReadCoachAI](https://github.com/Archer-hx/ReadCoachAI)

## Features

- Generate CEFR A1-C2 reading articles by language, topic, style, and target length.
- Read with original text, bilingual comparison, or sentence-by-sentence comparison.
- Hover on words for definitions, part of speech, grammar gender, and examples.
- Select a sentence to ask AI grammar questions or request rewrites in different styles.
- Generate vocabulary notes, grammar points, and multiple-choice comprehension quizzes.
- Save the latest 40 generated articles in browser `localStorage`.
- Run as a standalone HTML file with no build step and no server requirement.

## 功能亮点

- 按语言、题材、风格、词数和 CEFR 等级生成外语阅读文章。
- 支持原文、双栏对照、逐句对照三种阅读方式。
- 鼠标悬停单词即可查看释义、词性、语法性别和例句。
- 选中句子后可以向 AI 提问语法，也可以改写为不同表达风格。
- 自动生成词汇、语法要点和多选理解测验。
- 最近 40 篇文章保存在浏览器本地 `localStorage`。
- 单个 HTML 文件即可运行，不需要构建工具或后端服务。

## Quick Start

1. Open `ReadCoachAI.html` in a modern browser.
2. Get an API key from the [DeepSeek Open Platform](https://platform.deepseek.com/).
3. Click **API Key** in the right panel, enter your key, and choose a model.
4. Select the target language, CEFR level, article style, topic, and word count.
5. Click **生成文章** to generate the article, translation, analysis, and quiz.

## 快速开始

1. 用浏览器打开 `ReadCoachAI.html`。
2. 前往 [DeepSeek 开放平台](https://platform.deepseek.com/) 申请 API Key。
3. 点击右侧面板的 **API Key**，输入 Key 并选择模型。
4. 选择学习语言、CEFR 等级、文章风格、指定题材和目标词数。
5. 点击 **生成文章**，系统会依次生成文章、译文、分析和测验。

## Privacy

The project does not include any API key. The key entered by the user is stored only in browser `localStorage` and is sent directly to the DeepSeek API endpoint when requests are made.

本项目不内置任何 API Key。用户输入的 Key 只保存在浏览器本地 `localStorage` 中，请求时直接发送给 DeepSeek API。

## Repository Structure

```text
ReadCoachAI/
├── ReadCoachAI.html      # Standalone single-file app
├── src/                  # Split source version for development
│   ├── index.html
│   ├── css/
│   └── js/
├── README.md
├── NOTICE.md
└── LICENSE
```

The `src/` version should be served with a local static server, for example VS Code Live Server or `python -m http.server`. The standalone `ReadCoachAI.html` file can be opened directly.

## Tech Stack

- Pure HTML, CSS, and JavaScript
- DeepSeek chat completions API in an OpenAI-compatible format
- Server-Sent Events streaming
- Browser `localStorage`
- Google Fonts: DM Sans and Crimson Pro

## License

This project is released under the [MIT License](LICENSE). See [NOTICE.md](NOTICE.md) for project ownership and open-source attribution notes.
