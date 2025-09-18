# SvelteKit + TailwindCSS Template

A modern, ready-to-use template combining the power of SvelteKit with the utility-first styling of TailwindCSS. Perfect for rapidly building beautiful, performant web applications.

## ✨ Features

- 🏗️ **SvelteKit** - Full-stack framework with SSR, routing, and more
- 🎨 **TailwindCSS** - Utility-first CSS framework for rapid UI development
- 📘 **TypeScript** - Type safety and better developer experience
- ✅ **ESLint** - Code quality and consistency
- ⚡ **Vite** - Lightning-fast development and build tooling
- 📱 **Responsive Design** - Mobile-first approach

## 🚀 Getting Started

### Prerequisites

Make sure you have Node.js (version 18 or higher) installed on your machine.

### Installation

1. Clone this repository or use it as a template:
```sh
git clone <your-repo-url>
cd svelte-tailwindcss-template
```

2. Install dependencies:
```sh
npm install
# or
pnpm install
# or
yarn install
```

### Development

Start the development server:

```sh
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

The development server will be available at `http://localhost:5173`

## 🏗️ Project Structure

```
src/
├── routes/          # SvelteKit pages and API routes
│   ├── +layout.svelte
│   └── +page.svelte
├── lib/             # Reusable components and utilities
│   ├── index.ts
│   └── assets/
├── app.html         # HTML shell
├── app.css          # Global styles and TailwindCSS imports
└── app.d.ts         # Type definitions

static/              # Static assets
├── robots.txt
└── favicon.png
```

## 📦 Building

## 📦 Building

To create a production version of your app:

```sh
npm run build
```

You can preview the production build with:
```sh
npm run preview
```

> To deploy your app, you may need to install an [adapter](https://svelte.dev/docs/kit/adapters) for your target environment.

## 🎨 Using TailwindCSS

This template comes with TailwindCSS pre-configured. You can start using utility classes immediately:

```svelte
<div class="bg-blue-500 text-white p-4 rounded-lg shadow-md">
  <h1 class="text-2xl font-bold">Hello, TailwindCSS!</h1>
</div>
```

### Customizing Tailwind

- Modify `tailwind.config.js` to customize your design system
- Add custom styles in `src/app.css`
- Use the `@apply` directive for component-based styling

## 🛠️ Development Tips

### Adding New Pages
Create new routes by adding files to the `src/routes/` directory:
- `src/routes/about/+page.svelte` → `/about`
- `src/routes/blog/[slug]/+page.svelte` → `/blog/dynamic-slug`

### Components
Store reusable components in `src/lib/` and import them:
```svelte
<script>
  import MyComponent from '$lib/MyComponent.svelte';
</script>
```

### Styling
- Use TailwindCSS utility classes for rapid development
- Create component variants using Tailwind's `@apply` directive
- Leverage TailwindCSS IntelliSense in VS Code for better DX

## 📚 Learn More

- [SvelteKit Documentation](https://kit.svelte.dev/docs)
- [TailwindCSS Documentation](https://tailwindcss.com/docs)
- [Svelte Tutorial](https://svelte.dev/tutorial)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
