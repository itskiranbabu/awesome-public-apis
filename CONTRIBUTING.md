# Contributing to Awesome Public APIs

Thank you for your interest in contributing! This document provides guidelines for contributing to this project.

## 🎯 How to Contribute

### Adding a New API

1. **Fork the repository**
2. **Create a new branch**: `git checkout -b add-new-api`
3. **Add your API** to the appropriate category in README.md
4. **Follow the format** shown below
5. **Test the API** to ensure it works
6. **Submit a pull request**

### API Entry Format

```markdown
| [API Name](https://api-url.com) | Brief description | `authType` | Yes/No | Yes/No | Additional Info |
```

**Example:**
```markdown
| [OpenAI](https://platform.openai.com/docs) | GPT-4 and AI models | `apiKey` | Yes | Yes | [Example](#openai-example) |
```

### Required Information

- **API Name**: Official name with link to documentation
- **Description**: Clear, concise description (max 100 characters)
- **Auth**: Authentication type (`apiKey`, `OAuth`, `No`, etc.)
- **HTTPS**: Whether the API supports HTTPS (Yes/No)
- **CORS**: CORS support status (Yes/No/Unknown)

### Optional Enhancements

- Code examples in popular languages (JavaScript, Python, etc.)
- Use cases and real-world applications
- Rate limits and pricing information
- Quality ratings or popularity metrics

## 📋 Categories

APIs should be placed in the most appropriate category:

- 🤖 AI & Machine Learning
- 🔗 Blockchain & Cryptocurrency
- 🐾 Animals
- 🎨 Art & Design
- 📚 Books & Literature
- 💼 Business & Finance
- 📅 Calendar & Events
- ☁️ Cloud Storage
- 💱 Currency & Exchange
- 📊 Data & Analytics
- 🛠️ Development Tools
- 📧 Email & Communication
- 🎮 Entertainment & Gaming
- 🌍 Environment & Weather
- 🍔 Food & Drink
- 🏥 Health & Fitness
- 📰 News & Media
- 📸 Photography & Images
- 🗺️ Maps & Geocoding
- 🎵 Music & Audio
- 🔐 Security & Authentication
- 🛒 Shopping & E-commerce
- 📱 Social Media
- 🏃 Sports
- 🚗 Transportation
- 📹 Video & Streaming

If your API doesn't fit any category, suggest a new one in your PR!

## ✅ Quality Standards

### API Requirements

- ✅ Must be publicly accessible
- ✅ Must have documentation
- ✅ Must be actively maintained
- ✅ Should be free or have a free tier
- ✅ Should not require extensive setup

### Documentation Requirements

- Clear API endpoint structure
- Authentication instructions
- Request/response examples
- Rate limits clearly stated
- Error handling documentation

## 🔍 Testing Your Contribution

Before submitting, please:

1. **Verify the API link** works and points to documentation
2. **Test the API** with a simple request
3. **Check for duplicates** - ensure the API isn't already listed
4. **Validate formatting** - ensure markdown renders correctly
5. **Spell check** your contribution

## 📝 Code Examples

When adding code examples, follow these guidelines:

### JavaScript Example
```javascript
// Clear, commented code
const response = await fetch('https://api.example.com/endpoint', {
  headers: { 'Authorization': 'Bearer YOUR_API_KEY' }
});
const data = await response.json();
console.log(data);
```

### Python Example
```python
import requests

# Clear, commented code
response = requests.get('https://api.example.com/endpoint',
    headers={'Authorization': 'Bearer YOUR_API_KEY'})
data = response.json()
print(data)
```

### cURL Example
```bash
curl -X GET "https://api.example.com/endpoint" \
  -H "Authorization: Bearer YOUR_API_KEY"
```

## 🚫 What NOT to Include

- ❌ Deprecated or discontinued APIs
- ❌ APIs requiring paid-only access
- ❌ APIs with poor or no documentation
- ❌ Malicious or unethical APIs
- ❌ APIs that violate terms of service
- ❌ Duplicate entries

## 🎨 Style Guidelines

### Markdown Formatting

- Use proper heading levels (##, ###)
- Keep tables aligned and formatted
- Use emojis consistently with existing style
- Include blank lines between sections

### Writing Style

- Use clear, concise language
- Avoid marketing jargon
- Be objective and factual
- Use proper grammar and spelling

## 🔄 Pull Request Process

1. **Update README.md** with your changes
2. **Update the Table of Contents** if adding a new category
3. **Add code examples** if applicable
4. **Write a clear PR description** explaining your changes
5. **Link to API documentation** in the PR
6. **Wait for review** - maintainers will review within 48 hours

### PR Title Format

```
Add [API Name] to [Category]
```

**Example:**
```
Add Anthropic Claude to AI & Machine Learning
```

### PR Description Template

```markdown
## API Details
- **Name**: API Name
- **Category**: Category Name
- **Documentation**: https://api-docs-url.com
- **Free Tier**: Yes/No
- **Rate Limits**: X requests per minute

## Testing
- [ ] API link verified
- [ ] Documentation accessible
- [ ] Test request successful
- [ ] No duplicates found

## Additional Notes
Any additional context or information about the API.
```

## 🐛 Reporting Issues

Found a broken link or outdated information?

1. **Check existing issues** to avoid duplicates
2. **Create a new issue** with details:
   - API name and category
   - Problem description
   - Expected vs actual behavior
   - Screenshots if applicable

### Issue Template

```markdown
**API Name**: 
**Category**: 
**Issue Type**: [Broken Link / Outdated Info / Other]

**Description**:
Clear description of the issue

**Steps to Reproduce**:
1. Step one
2. Step two

**Expected Behavior**:
What should happen

**Actual Behavior**:
What actually happens
```

## 🌟 Recognition

Contributors will be:
- Listed in the README acknowledgments
- Credited in release notes
- Mentioned in social media updates

## 📞 Contact

Questions? Reach out:
- **GitHub Issues**: For bugs and feature requests
- **Discussions**: For general questions
- **Email**: contact@example.com

## 📜 Code of Conduct

### Our Pledge

We pledge to make participation in our project a harassment-free experience for everyone, regardless of:
- Age, body size, disability
- Ethnicity, gender identity
- Experience level
- Nationality, personal appearance
- Race, religion
- Sexual identity and orientation

### Our Standards

**Positive behavior:**
- Using welcoming and inclusive language
- Being respectful of differing viewpoints
- Gracefully accepting constructive criticism
- Focusing on what's best for the community

**Unacceptable behavior:**
- Trolling, insulting/derogatory comments
- Public or private harassment
- Publishing others' private information
- Other unethical or unprofessional conduct

## 🎓 Learning Resources

New to contributing? Check these out:
- [First Contributions](https://github.com/firstcontributions/first-contributions)
- [How to Contribute to Open Source](https://opensource.guide/how-to-contribute/)
- [GitHub Flow Guide](https://guides.github.com/introduction/flow/)

## 📊 Contribution Statistics

We track and celebrate contributions:
- Number of APIs added
- Code examples contributed
- Issues resolved
- Documentation improvements

## 🚀 Future Plans

We're always improving! Upcoming features:
- API testing automation
- Interactive API explorer
- Community ratings and reviews
- API comparison tools
- Integration tutorials

## 💡 Suggestions

Have ideas for improvement? We'd love to hear them!
- Open a discussion
- Create a feature request issue
- Join our community chat

---

**Thank you for contributing to Awesome Public APIs!** 🎉

Your contributions help developers worldwide discover and use amazing APIs.

*Last updated: December 29, 2025*