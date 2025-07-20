🎨 Screenshot to HTML Builder
Show Image
 Show Image
 Show Image
 Show Image
Transform your UI screenshots into clean, modern HTML and CSS code using AI. No backend required, works entirely in your browser!
✨ Features
🎯 Core Functionality
Drag & Drop Upload - Simple screenshot upload with visual feedback
AI-Powered Analysis - Uses OpenAI's GPT-4 Vision to understand UI layouts
Clean Code Generation - Produces semantic HTML and modern CSS
Live Preview - See your generated code in action immediately
Copy to Clipboard - One-click copying for immediate use
🎨 Modern Interface
Beautiful Design - Gradient backgrounds with smooth animations
Responsive Layout - Works perfectly on desktop, tablet, and mobile
Tabbed Code View - Separate tabs for HTML, CSS, and live preview
Real-time Feedback - Loading states, error handling, and success messages
Dark Code Theme - Syntax-highlighted code display
🔧 Technical Features
Client-Side Only - No server setup required, works from any browser
Zero Dependencies - Pure HTML, CSS, and JavaScript
Modern Web Standards - Uses latest browser APIs and best practices
Responsive Code Output - Generated code includes mobile-first responsive design
🚀 Quick Start
Option 1: Direct Download
Download or clone this repository
Open index.html in any modern browser
Enter your OpenAI API key
Upload a screenshot and generate HTML!
Option 2: Try Online
Visit my live demo https://mydavinci.netlify.app
📦 Installation
Prerequisites
Modern web browser (Chrome, Firefox, Safari, Edge)
OpenAI API key with GPT-4 Vision access
Local Setup
bash
# Clone the repository
git clone https://github.com/itzcharlie01/screenshot-to-HTML.git

# Navigate to the project directory
cd screenshot-to-html

# Open in your browser
open index.html
# or
python -m http.server 8000  # for local server
Static Hosting
Deploy to any static hosting service:
GitHub Pages: Push to gh-pages branch
Netlify: Drag and drop the HTML file
Vercel: Connect your repository
Surge.sh: surge . your-domain.com
🔧 Usage
Basic Usage
Get API Key: Visit OpenAI's platform and create an API key
Open Tool: Launch index.html in your browser
Enter API Key: Paste your OpenAI API key in the secure input field
Upload Screenshot: Drag and drop or browse for your UI screenshot
Generate Code: Click "Generate HTML" and wait for AI magic
Copy & Use: Use the tabbed interface to copy HTML, CSS, or view the live preview
Supported Image Types
PNG, JPG, JPEG, GIF, WebP
Maximum recommended size: 20MB
Works best with clear, high-contrast UI screenshots
Generated Code Features
The AI generates:
Semantic HTML with proper structure and accessibility
Modern CSS using Flexbox/Grid for layouts
Responsive design with mobile-first approach
Hover effects and interactive elements
Clean formatting ready for production use
🔐 Security & Privacy
API Key Security
⚠️ Important: Your API key is used directly in the browser
🔒 For Production: Consider implementing a backend proxy
💡 Recommendation: Use API keys with limited scope and budget limits
Privacy
Images are processed through OpenAI's API
No data is stored locally or on external servers
API key is only stored in browser memory (not persistent)
Production Deployment
For public hosting, consider this backend implementation:
javascript
// Optional backend for API key security
app.post('/api/generate-html', async (req, res) => {
  const response = await fetch('https://api.openai.com/v1/chat/completions', {
    method: 'POST',
    headers: {
      'Authorization': `Bearer ${process.env.OPENAI_API_KEY}`,
      'Content-Type': 'application/json'
    },
    body: JSON.stringify(req.body)
  });
  
  res.json(await response.json());
});
🎯 Use Cases
Perfect For
Rapid Prototyping - Convert mockups to code quickly
Learning HTML/CSS - See how designs translate to code
Client Presentations - Turn designs into interactive demos
Code Reviews - Generate starting points for manual refinement
Design System Documentation - Create code examples from components
Works Great With
Landing pages and marketing sites
Forms and input layouts
Card-based designs and dashboards
Navigation menus and headers
Button groups and UI components
Modal dialogs and overlays
🔨 Development
Project Structure
screenshot-to-html/
│
├── index.html          # Main application file
├── README.md          # This file
├── LICENSE            # MIT license
└── assets/            # Optional: screenshots, demos
Code Architecture
HTML Structure: Semantic layout with accessibility in mind
CSS Styling: Modern design with CSS custom properties
JavaScript: ES6+ with modern browser APIs
API Integration: Direct OpenAI API calls with error handling
Local Development
bash
# Serve locally (optional)
python -m http.server 8000
# or
npx serve .
# or
php -S localhost:8000
🤝 Contributing
We welcome contributions! Here's how you can help:
Ways to Contribute
🐛 Bug Reports: Open an issue with details and screenshots
💡 Feature Requests: Suggest new functionality or improvements
🔧 Code Contributions: Submit pull requests with enhancements
📚 Documentation: Help improve README, comments, or examples
Development Workflow
Fork the repository
Create a feature branch (git checkout -b feature/amazing-feature)
Make your changes
Test thoroughly
Commit your changes (git commit -m 'Add amazing feature')
Push to the branch (git push origin feature/amazing-feature)
Open a Pull Request
Code Style
Use consistent indentation (2 spaces)
Comment complex functionality
Follow semantic HTML principles
Use modern CSS practices
Keep JavaScript ES6+ compatible
📋 Roadmap
Planned Features
 Backend Option - Optional Express.js backend for API key security
 Multiple AI Models - Support for Claude, Gemini, and other vision models
 Code Optimization - Minification and optimization options
 Template Library - Pre-built component templates
 Batch Processing - Handle multiple screenshots at once
 Export Options - Download as ZIP, CodePen integration
 Dark Mode - Theme switching for the interface
 Code History - Save and manage generated code snippets
Version History
v1.0.0 - Initial release with core functionality
v1.1.0 - Planned: Enhanced error handling and validation
v1.2.0 - Planned: Multiple AI model support
⚠️ Known Limitations
API key visible in network requests (client-side limitation)
Dependent on OpenAI API availability and rate limits
Generated code may need manual refinement for complex designs
Large images may increase API costs and response times
🆘 Troubleshooting
Common Issues
API Key Error
Error: Invalid API key
Verify your API key is correct
Ensure you have GPT-4 Vision access
Check your OpenAI account billing status
Image Upload Issues
Error: Please select an image file
Confirm file is a valid image format
Try resizing if image is very large
Check browser console for additional errors
Generation Failures
Error: Failed to generate HTML
Check internet connection
Verify OpenAI service status
Try with a clearer, simpler screenshot
📝 License
This project is licensed under the MIT License - see the LICENSE file for details.
🙏 Acknowledgments
OpenAI for providing the GPT-4 Vision API
Modern CSS inspiration from contemporary web design trends
Open source community for best practices and patterns
🌟 Show Your Support
If this project helped you, please:
⭐ Star this repository
🍴 Fork and contribute
📢 Share with others
🐛 Report bugs and suggest features
<div align="center">
Made with ❤️ By Charlie for the developer community
Demo • Issues • Contribute
</div>
