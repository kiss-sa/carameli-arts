# Carameli Arts -- Portfolio Website

This website is a static website generated with Hugo to showcase the work of Carameli Arts as a personal portfolio.

## Theme colors & fonts

Colors and fonts are configured in [data/theme.json](data/theme.json). After editing it, regenerate `assets/css/generated-theme.css` with:

```
npm run theme:generate
```

or, to auto-regenerate on every save:

```
npm run theme:watch
```

Note: the theme's own `themes/roxo-hugo/scripts/themeGenerator.js` won't work directly in this project, since its setup detection looks for a `hugo.toml` and this site uses `hugo.yml`. [scripts/generate-theme-css.js](scripts/generate-theme-css.js) is a copy of that logic with paths hardcoded for this project instead.