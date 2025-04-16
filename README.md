# Parsel Hugo Theme

A modern Hugo theme powered by Tailwind CSS and daisyUI.

## Features

- Responsive design
- Dark mode / light mode toggle
- Tailwind CSS integration
- daisyUI components
- Mobile-friendly navigation
- Clean, readable typography
- Tags support

## Installation

### 1. Add the theme as a submodule

```bash
cd yourhugosite
git submodule add https://github.com/yourusername/parsel.git themes/parsel
```

### 2. Update your config file

In your site's config file (hugo.toml, config.yaml, or config.json), set the theme:

```toml
theme = "parsel"
```

### 3. Install npm dependencies

Navigate to the theme directory and install the dependencies:

```bash
cd themes/parsel
npm install
```

### 4. Build CSS files

For development (with watch mode):
```bash
npm run dev
```

For production build:
```bash
npm run build
```

## Configuration

Example configuration in your site's hugo.toml file:

```toml
baseURL = 'https://example.org/'
languageCode = 'en-US'
title = 'My Site Title'

# Theme settings
[params]
  # Enable dark mode toggle
  darkMode = true
  # Default theme (light, dark, or auto)
  defaultTheme = "light"
  # Main sections to show on homepage
  mainSections = ["posts"]

[[menus.main]]
name = 'Home'
pageRef = '/'
weight = 10

[[menus.main]]
name = 'Posts'
pageRef = '/posts'
weight = 20

[[menus.main]]
name = 'Tags'
pageRef = '/tags'
weight = 30
```

## Customizing the Theme

### Tailwind CSS

The theme uses Tailwind CSS for styling. You can customize the design by editing the `tailwind.config.js` file.

### daisyUI

The theme includes daisyUI for UI components. You can customize the daisyUI theme in the `tailwind.config.js` file:

```js
daisyui: {
  themes: ["light", "dark", "cupcake"], // Add only the themes you want to use
}
```

## License

MIT License
