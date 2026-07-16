# 🤝 Contributing

Thank you for your interest in contributing to this GitHub profile repository!

## How to Contribute

### Reporting Issues
- Found a broken link? Open an issue.
- Badge not rendering? Let me know.
- SVG display issue? Describe the browser and theme.

### Suggesting Improvements
- Open an issue with the `enhancement` label
- Describe the improvement and why it would be valuable
- Include mockups or examples if possible

### Pull Requests
1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-improvement`
3. Make your changes following the [Design System](./design-system.md)
4. Test SVGs render correctly in a browser
5. Submit a pull request with a clear description

## Guidelines

### SVG Standards
- Use vector shapes only — no raster images
- Use gradients, filters, masks as per design system
- Use reusable `<symbol>` and `<use>` elements
- Optimize: remove redundant attributes, minimize paths
- Test in GitHub's SVG renderer (push to a branch and view)

### Code Style
- Use consistent indentation (2 spaces) in SVG and YAML files
- Keep markdown clean and properly formatted
- Use relative paths for internal links (`./assets/...`)

### Commit Messages
Follow conventional commits:
```
feat: add new achievement to timeline
fix: correct broken badge URL
style: improve divider gradient colors
docs: update setup instructions
```

## Code of Conduct

Be respectful, constructive, and inclusive. This is a personal project, but collaboration is welcome.
