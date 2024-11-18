# WordPress Theme & Plugin Detector

🔍 A powerful, secure, and user-friendly tool to detect WordPress themes, plugins, and security vulnerabilities of any WordPress website. Built with PHP and modern JavaScript, featuring a clean and responsive UI with TailWinnd CSS.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Visit%20Site-blue)](https://yeasin.me/wordpress-theme-plugin-detector/)
[![GitHub License](https://img.shields.io/github/license/yeasinhossain/WPDetector)](https://github.com/yeasinhossain/WPDetector/blob/main/LICENSE)
[![PHP Version](https://img.shields.io/badge/PHP-%3E%3D7.4-blue.svg)](https://php.net/)

## 🌟 Features

- **Theme Detection**: Identify active themes and child themes
- **Plugin Discovery**: Detect installed WordPress plugins
- **Security Analysis**: Check for common security vulnerabilities
- **Version Information**: Display WordPress version details
- **Real-time Validation**: Instant URL validation and feedback
- **Secure Implementation**: Built with robust security measures
- **User-friendly Interface**: Clean, responsive design using Tailwind CSS

## 🚀 Live Demo

Visit the live tool: [WordPress Theme & Plugin Detector](https://yeasin.me/wordpress-theme-plugin-detector/)

## 🛠️ Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yeasinhossain/WPDetector.git
   ```

2. Move to your web server directory (e.g., htdocs for XAMPP):
   ```bash
   cd WPDetector
   ```

3. Ensure proper permissions for the cache directory:
   ```bash
   chmod 755 cache
   ```

4. Configure your web server to serve the application

## 💻 Requirements

- PHP 7.4 or higher
- Apache/Nginx web server
- mod_rewrite enabled
- curl extension
- json extension

## 🔒 Security Features

- XSS Protection
- CSRF Prevention
- Rate Limiting
- Input Validation
- Output Escaping
- Directory Traversal Prevention
- Secure File Operations
- SSL Certificate Verification

## 🎯 Usage

1. Enter the WordPress website URL you want to analyze
2. Click "Analyze" or press Enter
3. View detailed information about:
   - WordPress version
   - Active theme
   - Installed plugins
   - Security vulnerabilities
   - Recommendations

## 📝 API Documentation

### Endpoint

```
POST /check_wordpress.php
```

### Parameters

| Parameter | Type   | Required | Description            |
|-----------|--------|----------|------------------------|
| url       | string | Yes      | WordPress website URL  |

### Response Format

```json
{
    "isWordPress": true,
    "version": "x.x.x",
    "theme": {
        "name": "Theme Name",
        "version": "x.x.x",
        "author": "Author Name"
    },
    "plugins": [
        "plugin-name-1",
        "plugin-name-2"
    ],
    "security": {
        "version_exposed": boolean,
        "readme_exposed": boolean,
        "debug_log_accessible": boolean,
        "directory_listing": boolean
    }
}
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Credits

- Created by [Yeasin Hossain](https://yeasin.me)
- Powered by [PHP](https://php.net)
- Styled with [Tailwind CSS](https://tailwindcss.com)

## 📧 Contact

- Website: [yeasin.me](https://yeasin.me)
- GitHub: [@yeasinhossain](https://github.com/yeasinhossain)

## 🔄 Updates

- **v1.0.0** (2024)
  - Initial release
  - Core functionality implementation
  - Security features
  - Responsive design
