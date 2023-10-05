# VisionsNouvelles Starter Theme

### Theme setup
Clone git repository.
```
cd wp-content/themes
```
```
git clone https://gitlab.com/visions-nouvelles/wp_vn_starter_theme new_theme_slug
```
1. Set `VN_SLUG` value in `functions.php`
2. Set `load_theme_textdomain` value in `functions.php`
3. Set `Text Domain:` value in `style.css`
4. Change webpack.config.js `publicPath` theme slug.
5. Change webpack.config.js `proxy` and `host` values with your local domain.
6. Edit variables in `_bootstrap-core.scss` file.
7. Edit css variables in `template-tags.php` file in `vn_css_vars()` function.
8. Change gulpfile.js `path.dirname vn/` with theme slug.
9. Change gulpfile.js `vn.zip` with `{theme_slug}.zip`

### Project setup
Update package.json dependencies to latest.
```
npx npm-check-updates -u
```
Install dependencies.
```
npm install
```

### Compiles and hot-reloads for development
```
npm start
```

### Compiles and minifies for production
```
npm run build
```

### Zip theme files to desktop
```
gulp zip
```