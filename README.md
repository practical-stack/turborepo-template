# basecn-ui

> shadcn/ui components reimplemented with MUI Base UI

🚧 **Work in Progress** - This project is currently under active development

A drop-in alternative to shadcn/ui that uses MUI Base UI instead of Radix UI. Same components, same API, same developer experience - just a different foundation.

## Features

⚠️ **Note: Features listed below are planned - implementation is in progress**

- 🎨 **Unstyled by default** - Full control over styling and theming
- ♿ **Accessibility first** - Built with WAI-ARIA compliance in mind
- 🔧 **Highly customizable** - Easy to adapt to your design requirements
- 📦 **Copy & paste friendly** - No heavy dependencies, just copy what you need
- 🚀 **Built on MUI Base** - Leverages the robust foundation of MUI's headless components
- 💪 **TypeScript ready** - Full TypeScript support out of the box
- 🎯 **Developer focused** - Simple APIs that developers love to use

## Philosophy

basecn-ui provides the exact same components and API as shadcn/ui, but uses MUI Base UI as the underlying implementation instead of Radix UI. This means:

- 🔄 **Drop-in replacement** - Same component names, props, and usage patterns
- 🎯 **Identical developer experience** - If you know shadcn/ui, you know basecn-ui
- 🏗️ **Different foundation** - Powered by MUI Base UI for those who prefer it
- 📦 **Same philosophy** - Copy, paste, customize, and own your components

## Turborepo Monorepo Structure

This project is organized as a turborepo monorepo for efficient development and build processes:

### Development Commands

- **`pnpm dev`** - Start all apps in development mode
- **`pnpm build`** - Build all apps and packages
- **`pnpm lint`** - Run linting across all workspaces
- **`pnpm check-types`** - Type-check all TypeScript code
- **`pnpm format`** - Format code with Prettier

### Prerequisites

- **Node.js** >= 18
- **pnpm** 9.0.0 (specified as package manager)

The turborepo setup ensures efficient caching, parallel execution, and proper dependency management across the entire workspace.

## Development Status

🔨 **Currently in development** - Components are being actively implemented. Not ready for production use.

## Contributing

🚫 **Not accepting contributions at this time** - We're focusing on core development and will open up for contributions once the foundation is stable.

## License

Licensed under the [MIT license](./LICENSE.md).

## Acknowledgments

- [shadcn](https://github.com/shadcn) for creating the original shadcn/ui components and API design
- [base-ui](https://base-ui.com/react/overview/quick-start) for the excellent Base UI foundation
- The React community for continuous inspiration
