# Contributing to OpenCode Workspace

Thank you for your interest in contributing to this OpenCode workspace setup!

## 📋 Ways to Contribute

- Report bugs or issues with the setup scripts
- Suggest improvements to documentation
- Add support for additional platforms
- Share custom plugin configurations
- Improve installation scripts

## 🔧 Development Setup

1. Fork the repository
2. Clone your fork:
   ```bash
   git clone https://github.com/YOUR_USERNAME/workspace.git
   cd workspace
   ```
3. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```

## 📝 Guidelines

### Code Style

- Use clear, descriptive variable names
- Add comments for complex logic
- Follow existing script structure
- Test scripts on multiple platforms when possible

### Documentation

- Update README.md for major changes
- Keep PLUGINS.md in sync with plugin configurations
- Update SETUP_GUIDE.md for new installation steps
- Document new features in comments

### Commit Messages

Use clear, descriptive commit messages:
```
Add support for Windows installation

- Add Windows-specific setup script
- Update README with Windows instructions
- Test on Windows 10 and 11
```

## 🧪 Testing

Before submitting:

1. Test installation scripts:
   ```bash
   bash -n setup-environment.sh
   bash -n quick-start.sh
   ```

2. Validate JSON configuration:
   ```bash
   python3 -m json.tool .opencode/opencode.json
   python3 -m json.tool package.json
   ```

3. Verify documentation links work

4. Test on different platforms if possible:
   - Linux (Ubuntu, Fedora, etc.)
   - macOS (Intel, Apple Silicon)
   - Windows WSL

## 📚 Adding New Plugins

To add a new OpenCode plugin:

1. Update `.opencode/opencode.json`:
   ```json
   {
     "plugin": [
       "existing-plugin",
       "new-plugin-name"
     ]
   }
   ```

2. Add plugin configuration if needed:
   ```json
   {
     "plugins": {
       "new-plugin-name": {
         "enabled": true,
         "option": "value"
       }
     }
   }
   ```

3. Document in PLUGINS.md:
   - Description
   - Repository link
   - Key features
   - Installation steps
   - Configuration options
   - Usage examples

4. Update README.md with plugin mention

## 🐛 Reporting Issues

When reporting issues, include:

- Operating system and version
- Node.js version (`node --version`)
- OpenCode version (`opencode --version`)
- Error messages (full text)
- Steps to reproduce
- Expected vs actual behavior

## 💡 Suggesting Features

Open an issue with:

- Clear description of the feature
- Use case/motivation
- Proposed implementation (optional)
- Examples or mockups (if applicable)

## 🔒 Security

If you find a security issue:

- **Do not** open a public issue
- Email the maintainers privately
- Provide detailed description
- Wait for confirmation before disclosure

## 📜 Code of Conduct

- Be respectful and inclusive
- Welcome newcomers
- Focus on constructive feedback
- Keep discussions on-topic

## 🚀 Pull Request Process

1. Ensure your code follows guidelines
2. Update documentation
3. Test your changes
4. Create a pull request with:
   - Clear title and description
   - Reference to related issues
   - Summary of changes
   - Testing performed

5. Wait for review
6. Address feedback
7. Merge when approved

## 🎯 Priority Areas

We especially welcome contributions in:

- Windows native support (without WSL)
- Alternative shell support (fish, zsh, etc.)
- Plugin configuration examples
- Troubleshooting guides
- Video tutorials or guides
- Translations

## 📞 Contact

- GitHub Issues: Bug reports and feature requests
- GitHub Discussions: Questions and community chat
- Pull Requests: Code contributions

## 📄 License

By contributing, you agree that your contributions will be licensed under the same license as this project (see LICENSE file).

---

Thank you for contributing! 🎉
