# 🔢 AI Token Efficiency Tool: Format & Provider Comparison

A comprehensive web application that compares token efficiency between JSON, XML, YAML, and Markdown formats across multiple AI providers (OpenAI, Google Gemini, Anthropic Claude) for optimal API cost management.

## 🎯 Features

### Format Analysis
- **Real-time Format Conversion**: Automatically converts between JSON, XML, YAML, and Markdown formats
- **Token Analysis**: Compare both formatted and minified token counts
- **Multiple OpenAI Encodings**: Support for GPT-2, GPT-3, Codex, GPT-3.5/4, and GPT-4o encodings
- **Visual Token Breakdown**: See individual tokens with color coding and hover details

### Cross-Model Comparison
- **Multi-Provider Support**: Compare token counts across OpenAI, Google Gemini, and Anthropic Claude
- **Real API Integration**: Uses actual API endpoints for accurate token counting
- **Provider Optimization**: Identify which AI provider tokenizes your data most efficiently
- **Side-by-Side Comparison**: Large comparison table showing all formats and providers

### General Features
- **Example Data Sets**: 12 pre-built examples from simple to complex
- **API Key Management**: Secure localStorage for API keys with auto-loading
- **Cost Optimization**: Understand which format AND provider combination saves the most money
- **Tab-Based Interface**: Separate analysis modes for different use cases

## 🚀 Live Demo

Visit the live application: [Format Token Comparison Tool](https://wonderwhy-er.github.io/format-token-comparison/)

## 📊 What It Does

This tool helps developers optimize their AI API costs by comparing how the same data structure performs across different formats AND different AI providers:

### Format Comparison
- **JSON**: Standard web format, good balance of readability and efficiency
- **XML**: Verbose but structured, often less token-efficient
- **YAML**: Human-readable, varies in efficiency depending on structure
- **Markdown**: Human-readable documentation format, often very efficient

### Provider Comparison
- **OpenAI**: Uses tiktoken library for precise token counting
- **Google Gemini**: Real API integration with countTokens endpoint
- **Anthropic Claude**: Direct API calls using token counting endpoint

### Example Results
For typical user data across providers:

**Format Efficiency (OpenAI GPT-4o):**
- **JSON Formatted**: 32 tokens → **Minified**: 20 tokens (37.5% savings)
- **XML Formatted**: 55 tokens → **Minified**: 45 tokens (18.2% savings)  
- **YAML Formatted**: 19 tokens → **Minified**: 19 tokens (0% savings)
- **Markdown Formatted**: 15 tokens → **Minified**: 15 tokens (0% savings)

**Cross-Provider Comparison (JSON Minified):**
- **OpenAI GPT-4o**: 20 tokens
- **Google Gemini Pro**: 22 tokens
- **Anthropic Claude**: 18 tokens ← **Best choice!**

> **Note**: Google Gemini and Anthropic Claude APIs return the same token counts regardless of which model is selected within each provider.

## 🛠️ Built With

- **[js-tiktoken](https://github.com/dqbd/tiktoken)**: JavaScript port of OpenAI's tiktoken library
- **[js-yaml](https://github.com/nodeca/js-yaml)**: YAML parser and stringifier
- **Google Gemini API**: Real-time token counting via countTokens endpoint
- **Anthropic Claude API**: Direct token counting with CORS support
- **Vanilla JavaScript**: No frameworks, fast and lightweight
- **[Desktop Commander](https://desktopcommander.app/)**: Development environment

### API Integrations
- **OpenAI**: Client-side tokenization using tiktoken
- **Google Gemini**: `https://generativelanguage.googleapis.com/v1beta/models/{model}:countTokens`
- **Anthropic Claude**: `https://api.anthropic.com/v1/messages/count_tokens` with `anthropic-dangerous-direct-browser-access` header

## 💡 Use Cases

- **Multi-Provider Cost Optimization**: Choose the best format AND provider combination for lowest token costs
- **Format Migration**: Understand the token impact of changing data formats across different AI models
- **Provider Selection**: Compare how different AI providers tokenize your specific data structures  
- **Development Planning**: Estimate token costs for different data structures across providers
- **Educational**: Learn how different formats and providers affect tokenization
- **API Strategy**: Make informed decisions about which AI provider to use based on your data format

## 🎮 How to Use

### Format Analysis (Tab 1)
1. **Load an Example**: Choose from 12 pre-built examples or enter your own data
2. **Auto-Conversion**: Watch as data converts between JSON, XML, YAML, and Markdown formats
3. **Select Encoding**: Choose OpenAI encoding (GPT-2, GPT-3, GPT-4, GPT-4o)
4. **Analyze Results**: See formatted vs minified token counts in a clear table
5. **Visual Tokens**: Explore individual token breakdown with color coding and hover details

### Cross-Model Comparison (Tab 2)
1. **Enter API Keys**: Add your Google Gemini and/or Anthropic Claude API keys
   - Google Gemini: Get free key at [https://ai.google.dev](https://ai.google.dev)
   - Anthropic Claude: Get key at [https://console.anthropic.com](https://console.anthropic.com)
2. **Select Models**: Choose specific models from each provider (note: token counts are the same across models within each provider)
3. **Compare**: Click "Compare Across Models" to see side-by-side token counts
4. **Optimize**: Identify the best format + provider combination for your needs

### API Key Management
- **Auto-Save**: API keys are automatically saved to localStorage
- **Auto-Load**: Keys persist across browser sessions
- **Security**: Keys are stored locally and only sent to respective APIs

## 📁 Example Categories

### Small Examples
- Simple User Profile
- Product Information
- Basic Configuration
- API Response

### Medium Examples
- User Lists with Pagination
- E-commerce Orders
- Blog Posts with Comments
- Analytics Data

### Large Examples
- Company Database
- Survey Responses
- System Logs
- Complex Configurations

## 🔧 Local Development

1. Clone the repository:
```bash
git clone https://github.com/wonderwhy-er/format-token-comparison.git
cd format-token-comparison
```

2. Open `index.html` in your browser - that's it! No build process required.

## 📈 SEO & Performance

- Fully optimized for search engines with proper meta tags
- Open Graph and Twitter Card support for social sharing
- Schema.org structured data
- Fast loading with CDN-based dependencies
- Mobile-responsive design

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Add new example data sets
- Improve the UI/UX design
- Add support for more data formats (TOML, MessagePack, etc.)
- Enhance the token visualization features
- Add support for additional AI providers
- Improve API error handling and user feedback
- Add export functionality for comparison results

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- **OpenAI** for the original tiktoken library
- **[js-tiktoken](https://github.com/dqbd/tiktoken)** for the JavaScript port
- **[Desktop Commander](https://desktopcommander.app/)** for the development environment
- **Community** for feedback and suggestions

---

⚡ **Built with [Desktop Commander](https://desktopcommander.app/)** - The ultimate development environment for AI-powered coding.
