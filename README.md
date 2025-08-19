# 🔢 Format Token Comparison Tool

A powerful web application that compares token efficiency between JSON, XML, and YAML formats for OpenAI API cost optimization.

## 🎯 Features

- **Real-time Format Conversion**: Automatically converts between JSON, XML, and YAML formats
- **Token Analysis**: Compare both formatted and minified token counts
- **Multiple Encodings**: Support for GPT-2, GPT-3, Codex, GPT-3.5/4, and GPT-4o encodings
- **Visual Token Breakdown**: See individual tokens with color coding
- **Example Data Sets**: 12 pre-built examples from simple to complex
- **Cost Optimization**: Understand which format saves the most tokens (and money!)

## 🚀 Live Demo

Visit the live application: [Format Token Comparison Tool](https://fiberta.github.io/format-token-comparison/)

## 📊 What It Does

This tool helps developers optimize their OpenAI API costs by comparing how the same data structure performs across different formats:

- **JSON**: Standard web format, good balance of readability and efficiency
- **XML**: Verbose but structured, often less token-efficient
- **YAML**: Human-readable, varies in efficiency depending on structure

### Example Results
For typical user data:
- **JSON Formatted**: 32 tokens → **Minified**: 20 tokens (37.5% savings)
- **XML Formatted**: 55 tokens → **Minified**: 45 tokens (18.2% savings)  
- **YAML Formatted**: 19 tokens → **Minified**: 19 tokens (0% savings)

## 🛠️ Built With

- **[js-tiktoken](https://github.com/dqbd/tiktoken)**: JavaScript port of OpenAI's tiktoken library
- **[js-yaml](https://github.com/nodeca/js-yaml)**: YAML parser and stringifier
- **Vanilla JavaScript**: No frameworks, fast and lightweight
- **[Desktop Commander](https://desktopcommander.app/)**: Development environment

## 💡 Use Cases

- **API Cost Optimization**: Choose the most token-efficient format for your data
- **Format Migration**: Understand the token impact of changing data formats
- **Development Planning**: Estimate token costs for different data structures
- **Educational**: Learn how different formats affect tokenization

## 🎮 How to Use

1. **Load an Example**: Choose from 12 pre-built examples or enter your own data
2. **Auto-Conversion**: Watch as data converts between all three formats
3. **Analyze Results**: See formatted vs minified token counts in a clear table
4. **Visual Tokens**: Explore the individual token breakdown for each format
5. **Optimize**: Use insights to choose the most efficient format for your needs

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
git clone https://github.com/fiberta/format-token-comparison.git
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
- Improve the UI/UX
- Add support for more data formats
- Enhance the token visualization

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- **OpenAI** for the original tiktoken library
- **[js-tiktoken](https://github.com/dqbd/tiktoken)** for the JavaScript port
- **[Desktop Commander](https://desktopcommander.app/)** for the development environment
- **Community** for feedback and suggestions

---

⚡ **Built with [Desktop Commander](https://desktopcommander.app/)** - The ultimate development environment for AI-powered coding.
