# 🎨 Screenshot to HTML Builder

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Google Gemini](https://img.shields.io/badge/Powered%20by-Google%20Gemini-4285f4.svg)](https://ai.google.dev/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![No Backend](https://img.shields.io/badge/Backend-None%20Required-green.svg)](#)

> Transform your UI screenshots into clean, modern HTML and CSS code using Google Gemini AI. No backend required, works entirely in your browser!

**Made with ❤️ by Charles Ayere**

## ✨ Features

### 🎯 Core Functionality
- **Drag & Drop Upload** - Simple screenshot upload with visual feedback
- **AI-Powered Analysis** - Uses Google Gemini 1.5 Flash to understand UI layouts
- **Clean Code Generation** - Produces semantic HTML and modern CSS
- **Live Preview** - See your generated code in action immediately
- **Copy to Clipboard** - One-click copying for immediate use

### 🎨 Modern Interface
- **Beautiful Design** - Google-themed gradient backgrounds with smooth animations
- **Responsive Layout** - Works perfectly on desktop, tablet, and mobile
- **Tabbed Code View** - Separate tabs for HTML, CSS, and live preview
- **Real-time Feedback** - Loading states, error handling, and success messages
- **Dark Code Theme** - Syntax-highlighted code display

### 🔧 Technical Features
- **Client-Side Only** - No server setup required, works from any browser
- **Zero Dependencies** - Pure HTML, CSS, and JavaScript
- **Modern Web Standards** - Uses latest browser APIs and best practices
- **Responsive Code Output** - Generated code includes mobile-first responsive design

## 🚀 Quick Start

### Option 1: Direct Download
1. Download or clone this repository
2. Open `index.html` in any modern browser
3. Enter your Google AI API key (FREE!)
4. Upload a screenshot and generate HTML!

### Option 2: Try Online
Visit our [live demo](https://mydavinci.pages.dev)

## 📦 Installation

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- [Google AI Studio API key](https://aistudio.google.com/app/apikey) (FREE - no credit card required!)

### Local Setup
```bash
# Clone the repository
git clone https://github.com/itzcharlie01/screenshot-to-HTML.git

# Navigate to the project directory
cd screenshot-to-html

# Open in your browser
open index.html
# or
python -m http.server 8000  # for local server
```

### Static Hosting
Deploy to any static hosting service:
- **GitHub Pages**: Push to `gh-pages` branch
- **Netlify**: Drag and drop the HTML file
- **Vercel**: Connect your repository
- **Surge.sh**: `surge . your-domain.com`

## 🔧 Usage

### Basic Usage
1. **Get API Key**: Visit [Google AI Studio](https://aistudio.google.com/app/apikey) and create a FREE API key
2. **Open Tool**: Launch `index.html` in your browser
3. **Enter API Key**: Paste your Google AI API key (format: `AIza...`)
4. **Upload Screenshot**: Drag and drop or browse for your UI screenshot
5. **Generate Code**: Click "Generate HTML with Gemini" and watch the AI magic
6. **Copy & Use**: Use the tabbed interface to copy HTML, CSS, or view the live preview

### Supported Image Types
- PNG, JPG, JPEG, GIF, WebP
- Maximum recommended size: 20MB
- Works best with clear, high-contrast UI screenshots

### Generated Code Features
Gemini AI generates:
- **Semantic HTML** with proper structure and accessibility
- **Modern CSS** using Flexbox/Grid for layouts
- **Responsive design** with mobile-first approach
- **Hover effects** and interactive elements
- **Clean formatting** ready for production use
- **Color-accurate recreation** matching your original design

## 🆓 Why Google Gemini?

### Advantages Over Other AI Services
- **100% Free**: Generous free tier with no credit card required
- **No Waitlists**: Instant access to vision capabilities
- **Superior Vision**: Specifically excellent at understanding UI layouts
- **Fast Processing**: Quick response times for image analysis
- **Stable API**: Reliable service with clear error messages
- **Easy Setup**: Simple API key generation process

### API Comparison
| Feature | Google Gemini | OpenAI GPT-4V | Claude |
|---------|---------------|---------------|--------|
| **Cost** | 🟢 FREE tier | 🟡 Paid only | 🟡 Paid only |
| **Setup** | 🟢 Instant | 🟡 Waitlist | 🟡 Limited access |
| **UI Analysis** | 🟢 Excellent | 🟢 Very good | 🟢 Very good |
| **Rate Limits** | 🟢 Generous | 🟡 Restrictive | 🟡 Moderate |

## 🔐 Security & Privacy

### API Key Security
- ⚠️ **Important**: Your API key is used directly in the browser
- 🔒 **For Production**: Consider implementing a backend proxy
- 💡 **Recommendation**: Use API keys with limited scope and quota limits
- 🎯 **Good News**: Google AI Studio keys are free and easy to regenerate

### Privacy
- Images are processed through Google's Gemini API
- No data is stored locally or on external servers
- API key is only stored in browser memory (not persistent)
- Google's privacy policy applies to API usage

### Production Deployment
For public hosting, consider this backend implementation:

```javascript
// Optional backend for API key security
app.post('/api/generate-html', async (req, res) => {
  const response = await fetch(`https://generativelanguage.googleapis.com/v1beta/models/gemini-1.5-flash:generateContent?key=${process.env.GOOGLE_AI_API_KEY}`, {
    method: 'POST',
    headers: {
      'Content-Type': 'application/json'
    },
    body: JSON.stringify(req.body)
  });
  
  res.json(await response.json());
});
```

## 🎯 Use Cases

### Perfect For
- **Rapid Prototyping** - Convert mockups to code in seconds
- **Learning HTML/CSS** - See how designs translate to code
- **Client Presentations** - Turn static designs into interactive demos
- **Code Reviews** - Generate starting points for manual refinement
- **Design System Documentation** - Create code examples from components
- **Freelance Work** - Speed up development for client projects

### Works Great With
- Landing pages and marketing sites
- Forms and input layouts
- Card-based designs and dashboards
- Navigation menus and headers
- Button groups and UI components
- Modal dialogs and overlays
- E-commerce product pages
- Blog layouts and content sections

## 🔨 Development

### Project Structure
```
screenshot-to-html/
│
├── index.html          # Main application file
├── README.md          # This file
├── LICENSE            # MIT license
└── assets/            # Optional: screenshots, demos
```

### Code Architecture
- **HTML Structure**: Semantic layout with accessibility in mind
- **CSS Styling**: Google Material Design-inspired theme
- **JavaScript**: ES6+ with modern browser APIs
- **API Integration**: Direct Google Gemini API calls with robust error handling

### Local Development
```bash
# Serve locally (optional)
python -m http.server 8000
# or
npx serve .
# or
php -S localhost:8000
```

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### Ways to Contribute
- 🐛 **Bug Reports**: Open an issue with details and screenshots
- 💡 **Feature Requests**: Suggest new functionality or improvements
- 🔧 **Code Contributions**: Submit pull requests with enhancements
- 📚 **Documentation**: Help improve README, comments, or examples

### Development Workflow
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Test thoroughly with different image types
5. Commit your changes (`git commit -m 'Add amazing feature'`)
6. Push to the branch (`git push origin feature/amazing-feature`)
7. Open a Pull Request

### Code Style
- Use consistent indentation (2 spaces)
- Comment complex functionality
- Follow semantic HTML principles
- Use modern CSS practices
- Keep JavaScript ES6+ compatible
- Test with various image formats and sizes

## 📋 Roadmap

### Planned Features
- [ ] **Backend Option** - Optional Node.js backend for API key security
- [ ] **Multiple AI Models** - Support for OpenAI GPT-4V and Claude as alternatives
- [ ] **Code Optimization** - Minification and optimization options
- [ ] **Template Library** - Pre-built component templates
- [ ] **Batch Processing** - Handle multiple screenshots at once
- [ ] **Export Options** - Download as ZIP, CodePen integration
- [ ] **Dark Mode Toggle** - Theme switching for the interface
- [ ] **Code History** - Save and manage generated code snippets
- [ ] **Custom Prompts** - User-defined generation instructions
- [ ] **Component Detection** - Automatic UI component identification

### Version History
- **v1.0.0** - Initial release with Google Gemini integration
- **v1.1.0** - Planned: Enhanced error handling and validation
- **v1.2.0** - Planned: Multiple AI model support

## ⚠️ Known Limitations

- API key visible in network requests (client-side limitation)
- Dependent on Google Gemini API availability and rate limits
- Generated code may need manual refinement for complex designs
- Large images may increase processing time
- Some very complex layouts might require multiple iterations

## 🆘 Troubleshooting

### Common Issues

**API Key Error**
```
Error: Invalid API key
```
- Verify your API key is correct and starts with `AIza`
- Ensure you copied the complete key from Google AI Studio
- Check that your API key has Gemini model access enabled

**Permission Denied**
```
Error: Permission denied
```
- Make sure your Google AI Studio project is active
- Verify the API key hasn't expired
- Check your Google Cloud quota limits

**Image Upload Issues**
```
Error: Please select an image file
```
- Confirm file is a valid image format (PNG, JPG, etc.)
- Try resizing if image is very large (>20MB)
- Check browser console for additional errors

**Generation Failures**
```
Error: Failed to generate HTML
```
- Check internet connection
- Verify Google AI services status
- Try with a clearer, simpler screenshot
- Ensure image has good contrast and readable text

### Getting Help
- Check the [Google AI documentation](https://ai.google.dev/docs)
- Open an issue on GitHub with error details
- Try the debug steps in browser console (F12)

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Google AI Team** for providing the excellent Gemini API
- **Google Material Design** for design inspiration
- **Open source community** for best practices and patterns
- **Web development community** for feedback and suggestions

## 🌟 Show Your Support

If this project helped you, please:
- ⭐ Star this repository
- 🍴 Fork and contribute
- 📢 Share with other developers
- 🐛 Report bugs and suggest features
- 💬 Follow [@CharlesAyere](https://github.com/itzcharlie01) for updates

---

<div align="center">

**Made with ❤️ by Charlie for the developer community**

[Demo](https://mydavinci.pages.app) • [Issues](https://github.com/itzcharlie01/screenshot-to-HTML/issues) • [Contribute](https://github.com/itzcharlie01/screenshot-to-HTML/pulls)

Get your FREE Google AI API key: [Google AI Studio](https://aistudio.google.com/app/apikey)

</div>
