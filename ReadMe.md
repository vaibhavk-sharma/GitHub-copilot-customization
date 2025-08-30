# GitHub Copilot Customization

A comprehensive setup for customizing GitHub Copilot behavior with specialized instructions for a full-stack web application using React and Node.js.

## Project Structure

```
.github/
├── copilot-instructions.md    # Main project instructions
├── chatmodes/                 # Custom Copilot chat modes
├── instructions/              # Framework-specific guidelines
└── prompts/                   # Custom prompt templates
```

## Features

- **Project-wide Instructions**: Global coding standards and architectural guidelines. Please refer [copilot-instructions.md](.github/copilot-instructions.md)
- **Framework-specific Guidelines**:
  - React frontend development with Tailwind CSS. Please refer [react.instructions.md](.github/instructions/react.instructions.md)
  - Node.js/Express backend development. Please refer [node.instructions.md](.github/instructions/node.instructions.md)
- **Custom Chat Modes**: Specialized interaction modes for different development roles e.g. Architect. Please refer [architect.chatmode.md](.github/chatmodes/architect.chatmode.md)
- **Prompt Templates**: Reusable templates for common development tasks. Please refer files under [/prompts](.github/prompts) folder like: [react-component.prompt.md](.github/prompts/react-component.prompt.md)



## Getting Started

1. Clone this repository
2. Install GitHub Copilot in your IDE
3. The custom instructions will be automatically applied when working in this workspace

## References 
[Github Official Documentation to configure custom instructions for GitHub Copilot](https://docs.github.com/en/copilot/how-tos/configure-custom-instructions)