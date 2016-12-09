# Prosper App

The current version runs at [app.prosper.community](http://app.prosper.community)

## Introduction to Editing

1. After or while making changes you should run `grunt` which continuously
   updates the templates. The base directory is:
   ```
   /var/www/prosper-app
   ```
   the `grunt` process can be started relative to that:
   ```
   node_modules/grunt/bin/grunt
   ```
   once started it will watch the directory for changes.
2. Changes to CSS should be make to:
   ```
   styles/critical.css
   ```
   for now.
3. The connection to the backend is set in `js/lib/ic-module.js` line 22:
   ```
   icApiProvider.setBase('URL')
   ```
4. The URLs for specific API-calls are set in `js/lib/ic-api.js`.
5. Most of the language specific content comes from the backend (`/frontend/locale`).
6. Colors and icons are set in `styles/typography_and_colors.css`.
7. The home page can be found in `pages/main.html`. There are commented examples with tiles
   there.
