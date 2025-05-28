# Solo

Solo is a minimal theme for [Ghost](https://github.com/TryGhost/Ghost) focused on showcasing the work of an individual writer or creator. This theme is highly customizable, with a few simple settings that allow you to quickly apply your own personal style to your site.

**Demo: https://solo.ghost.io**

# Instructions

1. [Download this theme](https://github.com/TryGhost/Solo/archive/main.zip)
2. Log into Ghost, and go to the `Design` settings area to upload the zip file

# Development

Edition styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/), [Yarn](https://yarnpkg.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's root directory:

```bash
# Install
yarn

# Run build & watch for changes
yarn dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/solo.zip`, which you can then upload to your site.

```bash
yarn zip
```

# Contribution

This repo is synced automatically with [TryGhost/Themes](https://github.com/TryGhost/Themes) monorepo. If you're looking to contribute or raise an issue, head over to the main repository [TryGhost/Themes](https://github.com/TryGhost/Themes) where our official themes are developed.

## Copyright & License

Copyright (c) 2013-2025 Ghost Foundation - Released under the [MIT license](LICENSE).

# Brand Guide Plan

1.  **Understand Nordvik's Brand:** We'll need to understand the core brand elements of Nordvik and its associated brands. This includes logos, color palettes, typography, tone of voice, and any specific style guidelines.

2.  **Adapt the "Solo" Theme:** We'll modify the "Solo" theme to reflect Nordvik's branding. This will involve:
    *   **Replacing assets:** Swapping out default images, fonts, and potentially other assets with Nordvik's.
    *   **Updating CSS:** Adjusting the stylesheet (`assets/css/screen.css`) to implement Nordvik's color palette, typography, and layout preferences. We've started implementing dark mode using CSS variables in this step.
    *   **Modifying templates:** Making changes to the theme's Handlebars templates (`.hbs` files) to accommodate any specific structural or content requirements for the brand guide. This might involve adding new sections or modifying existing ones to better suit the purpose of showcasing brand guidelines.

3.  **Create Brand Guide Content Structure:** We'll need to define a clear structure for the brand guide content within the Ghost CMS. This could involve using tags, pages, or a combination of both to organize guidelines for different brands or aspects of the brand.

4.  **Develop Customizations (if needed):** If the standard Ghost features and theme modifications aren't sufficient, we might explore custom Ghost theme development to add specific functionalities or content types required for the brand guide.

5.  **Testing and Refinement:** Throughout the process, we'll test the modified theme on your Ghost CMS instance to ensure everything is working correctly and the branding is consistently applied. We'll refine the theme and content based on feedback and testing.

6.  **Documentation:** We'll document the changes we've made to the theme and provide instructions on how to use it to create and manage the brand guide content within Ghost.

7.  **Implement Dark Mode Toggle:** We'll add an HTML element for the dark mode toggle switch to the theme's Handlebars files. We'll then add the final JavaScript code to `assets/js/main.js` to handle the toggle functionality, including saving the user's preference to local storage so it persists across sessions.

