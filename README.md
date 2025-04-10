## SIDHE Token Design System 

## Project Overview
## Project Structure 
# SIDHE Design System - Project Structure

```
sidhe-design-system/
├── README.md
├── package.json
├── config.js
│
├── tokens/
│   ├── colors.json
│   ├── typography.json
│   ├── spacing.json
│   ├── radius.json
│   ├── effects.json
│   └── stroke.json
│
├── platforms/
│   ├── web/
│   │   ├── css/
│   │   │   └── sidhe-tokens.css
│   │   └── scss/
│   │       └── _sidhe-tokens.scss
│   │
│   ├── android/
│   │   └── res/
│   │       └── values/
│   │           ├── sidhe_colors.xml
│   │           ├── sidhe_dimens.xml
│   │           ├── sidhe_typography.xml
│   │           └── sidhe_styles.xml
│   │
│   └── ios/
│       └── SIDHEDesignSystem/
│           ├── Sources/
│           │   ├── SIDHEColors.swift
│           │   ├── SIDHETypography.swift
│           │   ├── SIDHESpacing.swift
│           │   └── SIDHEComponents.swift
│           └── Package.swift
│
├── examples/
│   ├── web/
│   │   ├── index.html
│   │   └── components.html
│   │
│   ├── android/
│   │   └── app/
│   │       └── src/main/
│   │           ├── java/
│   │           └── res/layout/
│   │               └── activity_main.xml
│   │
│   └── ios/
│       └── SIDHEExample/
│           └── ContentView.swift
│
├── .github/
│   └── workflows/
│       └── build-tokens.yml
│
└── dist/
    ├── web/
    │   ├── css/
    │   └── scss/
    │
    ├── android/
    │   └── res/
    │
    └── ios/
        └── SIDHEDesignSystem/
```

## Token Structure 
## SIDHE Design Tokens Structure

### colors.json
```json
{
  "color": {
    "primary": {
      "100": { "value": "#F686C2", "type": "color" },
      "200": { "value": "#F45BB6", "type": "color" },
      "300": { "value": "#F233AB", "type": "color" },
      "400": { "value": "#EF0A9F", "type": "color" },
      "500": { "value": "#EC0094", "type": "color" },
      "10": { "value": "rgba(236, 0, 148, 0.1)", "type": "color" }
    },
    "secondary": {
      "100": { "value": "#A888E5", "type": "color" },
      "200": { "value": "#8C59DD", "type": "color" },
      "300": { "value": "#702BD5", "type": "color" },
      "400": { "value": "#5500CC", "type": "color" },
      "500": { "value": "#3A0099", "type": "color" },
      "10": { "value": "rgba(58, 0, 153, 0.1)", "type": "color" }
    },
    "neutral": {
      "100": { "value": "#F5F5F5", "type": "color" },
      "200": { "value": "#E0E0E0", "type": "color" },
      "300": { "value": "#BDBDBD", "type": "color" },
      "400": { "value": "#9E9E9E", "type": "color" },
      "500": { "value": "#757575", "type": "color" },
      "600": { "value": "#616161", "type": "color" },
      "700": { "value": "#424242", "type": "color" },
      "800": { "value": "#303030", "type": "color" },
      "900": { "value": "#212121", "type": "color" },
      "1000": { "value": "#121212", "type": "color" },
      "10": { "value": "rgba(33, 33, 33, 0.1)", "type": "color" }
    },
    "red": {
      "100": { "value": "#FF5A5A", "type": "color" },
      "200": { "value": "#DD0E10", "type": "color" },
      "10": { "value": "rgba(221, 14, 16, 0.1)", "type": "color" }
    },
    "yellow": {
      "100": { "value": "#FFDE59", "type": "color" },
      "200": { "value": "#C9AB19", "type": "color" },
      "10": { "value": "rgba(201, 171, 25, 0.1)", "type": "color" }
    },
    "green": {
      "100": { "value": "#56E0B2", "type": "color" },
      "200": { "value": "#17AF66", "type": "color" },
      "10": { "value": "rgba(23, 175, 102, 0.1)", "type": "color" }
    }
  }
}
```

### typography.json
```json
{
  "font": {
    "family": {
      "primary": { "value": "Plus Jakarta Sans, sans-serif", "type": "fontFamily" },
      "secondary": { "value": "Lora, serif", "type": "fontFamily" }
    },
    "weight": {
      "regular": { "value": "400", "type": "fontWeight" },
      "medium": { "value": "500", "type": "fontWeight" },
      "semiBold": { "value": "600", "type": "fontWeight" },
      "bold": { "value": "700", "type": "fontWeight" }
    },
    "size": {
      "xs": { "value": "12px", "type": "fontSize" },
      "sm": { "value": "14px", "type": "fontSize" },
      "md": { "value": "16px", "type": "fontSize" },
      "lg": { "value": "18px", "type": "fontSize" },
      "xl": { "value": "20px", "type": "fontSize" },
      "2xl": { "value": "24px", "type": "fontSize" },
      "3xl": { "value": "30px", "type": "fontSize" },
      "4xl": { "value": "36px", "type": "fontSize" },
      "5xl": { "value": "48px", "type": "fontSize" },
      "6xl": { "value": "60px", "type": "fontSize" }
    },
    "lineHeight": {
      "none": { "value": "1", "type": "lineHeight" },
      "tight": { "value": "1.25", "type": "lineHeight" },
      "snug": { "value": "1.375", "type": "lineHeight" },
      "normal": { "value": "1.5", "type": "lineHeight" },
      "relaxed": { "value": "1.625", "type": "lineHeight" },
      "loose": { "value": "2", "type": "lineHeight" }
    },
    "letterSpacing": {
      "tighter": { "value": "-0.05em", "type": "letterSpacing" },
      "tight": { "value": "-0.025em", "type": "letterSpacing" },
      "normal": { "value": "0", "type": "letterSpacing" },
      "wide": { "value": "0.025em", "type": "letterSpacing" },
      "wider": { "value": "0.05em", "type": "letterSpacing" },
      "widest": { "value": "0.1em", "type": "letterSpacing" }
    }
  }
}
```

### spacing.json
```json
{
  "spacing": {
    "0": { "value": "0px", "type": "spacing" },
    "1": { "value": "4px", "type": "spacing" },
    "2": { "value": "8px", "type": "spacing" },
    "3": { "value": "12px", "type": "spacing" },
    "4": { "value": "16px", "type": "spacing" },
    "5": { "value": "20px", "type": "spacing" },
    "6": { "value": "24px", "type": "spacing" },
    "8": { "value": "32px", "type": "spacing" },
   }
  }
```


### Style Dictionary Configuration (config.json)
const StyleDictionary = require('style-dictionary');

// Custom transforms
StyleDictionary.registerTransform({
  name: 'size/px',
  type: 'value',
  matcher: (token) => {
    return typeof token.value === 'string' && token.value.endsWith('px');
  },
  transformer: (token) => {
    return parseFloat(token.value.replace('px', ''));
  }
});

// Base configuration
module.exports = {
  source: ['tokens/**/*.json'],
  platforms: {
    // Web: CSS Variables
    css: {
      transformGroup: 'css',
      buildPath: 'dist/web/css/',
      files: [{
        destination: 'sidhe-tokens.css',
        format: 'css/variables',
        options: {
          selector: ':root',
          outputReferences: true
        }
      }]
    },
    
    // Web: SCSS Variables
    scss: {
      transformGroup: 'scss',
      buildPath: 'dist/web/scss/',
      files: [{
        destination: '_sidhe-tokens.scss',
        format: 'scss/variables',
        options: {
          outputReferences: true
        }
      }]
    },
    
    // Android: XML Resources
    android: {
      transforms: ['attribute/cti', 'name/cti/kebab', 'size/density', 'color/hex'],
      buildPath: 'dist/android/res/values/',
      files: [
        {
          destination: 'sidhe_colors.xml',
          format: 'android/colors',
          filter: { type: 'color' }
        },
        {
          destination: 'sidhe_dimens.xml',
          format: 'android/dimens',
          filter: {
            attributes: { type: ['spacing', 'borderRadius', 'fontSize'] }
          }
        }
      ]
    },
    
    // iOS: Swift Constants
    ios: {
      transformGroup: 'ios',
      buildPath: 'dist/ios/Sources/',
      files: [
        {
          destination: 'SIDHEColors.swift',
          format: 'ios/swift/enum.swift',
          className: 'SIDHEColors',
          filter: { type: 'color' }
        },
        {
          destination: 'SIDHETypography.swift',
          format: 'ios/swift/enum.swift',
          className: 'SIDHETypography',
          filter: { attributes: { category: 'font' } }
        }
      ]
    }
  }
};

## Package.json with Automation Scripts
{
  "name": "sidhe-design-system",
  "version": "1.0.0",
  "description": "SIDHE Design System Tokens and Components",
  "main": "dist/js/index.js",
  "files": [
    "dist"
  ],
  "scripts": {
    "clean": "rimraf dist",
    "lint": "eslint .",
    "format": "prettier --write \"**/*.{js,json,md}\"",
    
    "build": "npm run clean && npm run build:tokens && npm run build:docs",
    "build:tokens": "style-dictionary build --config ./config.js",
    "build:web": "style-dictionary build --config ./config.js --platform css,scss,js",
    "build:android": "style-dictionary build --config ./config.js --platform android",
    "build:ios": "style-dictionary build --config ./config.js --platform ios",
    
    "build:docs": "npm run build:storybook",
    "build:storybook": "build-storybook -c .storybook -o dist/storybook",
    
    "start": "npm run start:storybook",
    "start:storybook": "start-storybook -p 6006",
    
    "test": "jest",
    "test:watch": "jest --watch",
    "test:coverage": "jest --coverage",
    
    "version": "auto-changelog -p && git add CHANGELOG.md",
    "preversion": "npm run test",
    "postversion": "git push && git push --tags",
    
    "publish:tokens": "npm run build:tokens && npm publish --access public",
    "publish:docs": "npm run build:docs && gh-pages -d dist/storybook",
    
    "watch": "npm-watch",
    "validate:tokens": "node ./scripts/validate-tokens.js"
  },
  "watch": {
    "build:tokens": {
      "patterns": ["tokens/**/*.json"],
      "extensions": "json"
    },
    "build:docs": {
      "patterns": ["docs/**/*", "examples/**/*"],
      "extensions": "md,js,jsx"
    }
  },
  "husky": {
    "hooks": {
      "pre-commit": "lint-staged",
      "pre-push": "npm run test"
    }
  },
  "lint-staged": {
    "*.{js,jsx}": ["eslint --fix", "prettier --write"],
    "*.{json,md}": ["prettier --write"]
  },
  "keywords": [
    "design-system",
    "tokens",
    "sidhe",
    "style-dictionary",
    "css",
    "scss",
    "android",
    "ios"
  ],
  "author": "SIDHE Design Team",
  "license": "MIT",
  "repository": {
    "type": "git",
    "url": "git+https://github.com/sidhe/design-system.git"
  },
  "bugs": {
    "url": "https://github.com/sidhe/design-system/issues"
  },
  "homepage": "https://sidhe.github.io/design-system",
  "dependencies": {
    "style-dictionary": "^3.8.0"
  },
  "devDependencies": {
    "@babel/core": "^7.22.5",
    "@babel/preset-env": "^7.22.5",
    "@storybook/addon-actions": "^7.0.20",
    "@storybook/addon-essentials": "^7.0.20",
    "@storybook/addon-links": "^7.0.20",
    "@storybook/react": "^7.0.20",
    "auto-changelog": "^2.4.0",
    "babel-loader": "^9.1.2",
    "eslint": "^8.42.0",
    "eslint-config-prettier": "^8.8.0",
    "gh-pages": "^5.0.0",
    "husky": "^8.0.3",
    "jest": "^29.5.0",
    "lint-staged": "^13.2.2",
    "npm-watch": "^0.11.0",
    "prettier": "^2.8.8",
    "rimraf": "^5.0.1"
  },
  "engines": {
    "node": ">=14.0.0"
  }
}
## Github Actions Workflow 
name: Build and Deploy Design Tokens

on:
  push:
    branches: [ main ]
    paths:
      - 'tokens/**'
      - 'config.js'
      - 'package.json'
      - '.github/workflows/build-tokens.yml'
  pull_request:
    branches: [ main ]
    paths:
      - 'tokens/**'
      - 'config.js'
  workflow_dispatch:
    inputs:
      environment:
        description: 'Environment to deploy to'
        required: true
        default: 'production'
        type: choice
        options:
          - production
          - staging

jobs:
  validate:
    name: Validate Tokens
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v3

      - name: Setup Node.js
        uses: actions/setup-node@v3
        with:
          node-version: '16'
          cache: 'npm'

      - name: Install dependencies
        run: npm ci

      - name: Validate token structure
        run: npm run validate:tokens

  build:
    name: Build Tokens
    needs: validate
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v3

      - name: Setup Node.js
        uses: actions/setup-node@v3
        with:
          node-version: '16'
          cache: 'npm'

      - name: Install dependencies
        run: npm ci

      - name: Build tokens for all platforms
        run: npm run build:tokens

      - name: Upload build artifacts
        uses: actions/upload-artifact@v3
        with:
          name: token-distribution
          path: dist/
          retention-days: 7

  test:
    name: Test Token Output
    needs: build
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v3

      - name: Setup Node.js
        uses: actions/setup-node@v3
        with:
          node-version: '16'
          cache: 'npm'

      - name: Install dependencies
        run: npm ci

      - name: Download build artifacts
        uses: actions/download-artifact@v3
        with:
          name: token-distribution
          path: dist/

      - name: Run tests
        run: npm test

  deploy-npm:
    name: Publish to NPM
    needs: test
    if: github.event_name == 'push' || github.event.inputs.environment == 'production'
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v3

      - name: Setup Node.js
        uses: actions/setup-node@v3
        with:
          node-version: '16'
          registry-url: 'https://registry.npmjs.org'
          cache: 'npm'

      - name: Install dependencies
        run: npm ci

      - name: Download build artifacts
        uses: actions/download-artifact@v3
        with:
          name: token-distribution
          path: dist/

      - name: Publish to NPM
        run: |
          if [[ $GITHUB_REF == refs/tags/v* ]]; then
            npm publish
          else
            npm publish --tag next
          fi
        env:
          NODE_AUTH_TOKEN: ${{ secrets.NPM_TOKEN }}

  deploy-docs:
    name: Deploy Documentation
    needs: test
    if: github.event_name == 'push' || github.event.inputs.environment == 'production'
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v3

      - name: Setup Node.js
        uses: actions/setup-node@v3
        with:
          node-version: '16'
          cache: 'npm'

      - name: Install dependencies
        run: npm ci

      - name: Download build artifacts
        uses: actions/download-artifact@v3
        with:
          name: token-distribution
          path: dist/

      - name: Build documentation
        run: npm run build:docs

      - name: Deploy to GitHub Pages
        uses: JamesIves/github-pages-deploy-action@v4.4.1
        with:
          branch: gh-pages
          folder: dist/storybook
          clean: true

  create-release:
    name: Create GitHub Release
    needs: [deploy-npm, deploy-docs]
    if: startsWith(github.ref, 'refs/tags/v')
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v3
        with:
          fetch-depth: 0

      - name: Download build artifacts
        uses: actions/download-artifact@v3
        with:
          name: token-distribution
          path: dist/

      - name: Zip artifacts
        run: |
          zip -r sidhe-tokens-android.zip dist/android
          zip -r sidhe-tokens-ios.zip dist/ios
          zip -r sidhe-tokens-web.zip dist/web
          zip -r sidhe-tokens-all.zip dist/

      - name: Generate Release Notes
        run: |
          echo "# SIDHE Design System Release" > RELEASE_NOTES.md
          echo "## Changes in this release" >> RELEASE_NOTES.md
          git log $(git describe --tags --abbrev=0 HEAD^)..HEAD --pretty=format:"- %s" >> RELEASE_NOTES.md

      - name: Create GitHub Release
        uses: softprops/action-gh-release@v1
        with:
          files: |
            sidhe-tokens-android.zip
            sidhe-tokens-ios.zip
            sidhe-tokens-web.zip
            sidhe-tokens-all.zip
          body_path: RELEASE_NOTES.md
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          
## Full Dictionary 

## Color 
/* ===== 1. COLORS ===== */
// colors.xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <!-- Primary Colors -->
    <color name="figr_color_primary_100">#FFF686C2</color>
    <color name="figr_color_primary_200">#FFF45BB6</color>
    <color name="figr_color_primary_300">#FFF233AB</color>
    <color name="figr_color_primary_400">#FFEF0A9F</color>
    <color name="figr_color_primary_500">#FFEC0094</color>
    <color name="figr_color_primary_10">#1AEC0094</color>

    <!-- Secondary Colors -->
    <color name="figr_color_secondary_100">#FFA888E5</color>
    <color name="figr_color_secondary_200">#FF8C59DD</color>
    <color name="figr_color_secondary_300">#FF702BD5</color>
    <color name="figr_color_secondary_400">#FF5500CC</color>
    <color name="figr_color_secondary_500">#FF3A0099</color>
    <color name="figr_color_secondary_10">#1A3A0099</color>

    <!-- Neutral Colors -->
    <color name="figr_color_neutral_100">#FFF5F5F5</color>
    <color name="figr_color_neutral_200">#FFE0E0E0</color>
    <color name="figr_color_neutral_300">#FFBDBDBD</color>
    <color name="figr_color_neutral_400">#FF9E9E9E</color>
    <color name="figr_color_neutral_500">#FF757575</color>
    <color name="figr_color_neutral_600">#FF616161</color>
    <color name="figr_color_neutral_700">#FF424242</color>
    <color name="figr_color_neutral_800">#FF303030</color>
    <color name="figr_color_neutral_900">#FF212121</color>
    <color name="figr_color_neutral_1000">#FF121212</color>
    <color name="figr_color_neutral_10">#1A212121</color>

    <!-- Feedback Colors -->
    <color name="figr_color_red_100">#FFFF5A5A</color>
    <color name="figr_color_red_200">#FFDD0E10</color>
    <color name="figr_color_red_10">#1ADD0E10</color>

    <color name="figr_color_yellow_100">#FFFFDE59</color>
    <color name="figr_color_yellow_200">#FFC9AB19</color>
    <color name="figr_color_yellow_10">#1AC9AB19</color>

    <color name="figr_color_green_100">#FF56E0B2</color>
    <color name="figr_color_green_200">#FF17AF66</color>
    <color name="figr_color_green_10">#1A17AF66</color>
    
    <!-- Third Color - Lime -->
    <color name="figr_color_thirdColor_100">#FFF8FAD2</color>
    <color name="figr_color_thirdColor_200">#FFE6F746</color>
    <color name="figr_color_thirdColor_300">#FFC6DC26</color>
    <color name="figr_color_thirdColor_400">#FFA6C106</color>
    <color name="figr_color_thirdColor_500">#FF859C05</color>
    <color name="figr_color_thirdColor_10">#1A859C05</color>
    <color name="figr_color_thirdColor_50">#80C6DC26</color>
</resources>

## Typography 
// 2. TYPOGRAPHY TOKENS
const FigrTypography = {
  // Font Families
  fontFamilies: {
    primary: "Plus Jakarta Sans, sans-serif",
    secondary: "Lora, serif"
  },
  
  // Font Weights
  fontWeights: {
    regular: 400,
    medium: 500,
    semiBold: 600,
    bold: 700
  },
  
  // Font Sizes
  fontSizes: {
    base: "16px",
    xs: "12px",    // 0.75rem
    sm: "14px",    // 0.875rem
    md: "16px",    // 1rem
    lg: "18px",    // 1.125rem
    xl: "20px",    // 1.25rem
    "2xl": "24px", // 1.5rem
    "3xl": "30px", // 1.875rem
    "4xl": "36px", // 2.25rem
    "5xl": "48px", // 3rem
    "6xl": "60px"  // 3.75rem
  },
  
  // Line Heights
  lineHeights: {
    none: 1,
    tight: 1.25,
    snug: 1.375,
    normal: 1.5,
    relaxed: 1.625,
    loose: 2
  },
  
  // Letter Spacing
  letterSpacing: {
    tighter: "-0.05em",
    tight: "-0.025em",
    normal: "0",
    wide: "0.025em",
    wider: "0.05em",
    widest: "0.1em"
  },
  
  // Text Styles (Compositions)
  textStyles: {
    // Headings
    heading1: {
      fontFamily: "Lora, serif",
      fontSize: "48px",
      fontWeight: 700,
      lineHeight: 1.25
    },
    heading2: {
      fontFamily: "Lora, serif",
      fontSize: "36px",
      fontWeight: 700,
      lineHeight: 1.25
    },
    heading3: {
      fontFamily: "Lora, serif",
      fontSize: "30px",
      fontWeight: 600,
      lineHeight: 1.25
    },
    // Body Text
    body: {
      fontFamily: "Plus Jakarta Sans, sans-serif",
      fontSize: "16px",
      fontWeight: 400,
      lineHeight: 1.5
    },
    bodySmall: {
      fontFamily: "Plus Jakarta Sans, sans-serif",
      fontSize: "14px",
      fontWeight: 400,
      lineHeight: 1.5
    },
    caption: {
      fontFamily: "Plus Jakarta Sans, sans-serif",
      fontSize: "12px",
      fontWeight: 400,
      lineHeight: 1.5
    }
  }
};
## Effects
// 3. EFFECT TOKENS
const FigrEffects = {
  // Shadow Effects
  elevation: {
    e0: "none",
    e1: "0px 1px 2px rgba(0, 0, 0, 0.05), 0px 1px 3px rgba(0, 0, 0, 0.1)",
    e2: "0px 2px 4px rgba(0, 0, 0, 0.05), 0px 3px 6px rgba(0, 0, 0, 0.1)",
    e3: "0px 4px 8px rgba(0, 0, 0, 0.05), 0px 6px 12px rgba(0, 0, 0, 0.1)"
  },
  
  // Inset/Sunken Effects
  sunken: {
    sm: "inset 0px 1px 2px rgba(0, 0, 0, 0.05)",
    md: "inset 0px 2px 4px rgba(0, 0, 0, 0.1)"
  },
  
  // Glow Effects
  glow: {
    sm: "0px 0px 4px rgba(236, 0, 148, 0.2)",
    md: "0px 0px 8px rgba(236, 0, 148, 0.3)",
    lg: "0px 0px 16px rgba(236, 0, 148, 0.4)"
  },
  
  // Effect Styles
  styles: {
    softDiffusion: {
      name: "Soft Diffusion",
      description: "Gentle, understated quality creating warmth and sophistication",
      filter: "blur(8px)",
      opacity: 0.8
    },
    strongDiffusion: {
      name: "Strong Diffusion",
      description: "Sharper, more defined edges adding clarity and precision",
      filter: "blur(4px)",
      opacity: 0.9
    },
    neobrutalism: {
      name: "Neobrutalism",
      description: "Bold, unapologetic aesthetic with bright colors and strong effects",
      boxShadow: "4px 4px 0px rgba(0, 0, 0, 0.9)",
      border: "2px solid #000"
    }
  }
};

## Radius 
// 4. RADIUS TOKENS
const FigrRadius = {
  base0: "0px", // Sharp edge - precise, formal aesthetic
  base2: "2px", // Very subtle
  base4: "4px", // Subtle
  base8: "8px", // Medium - balanced approach
  base12: "12px", // Prominent
  baseRound: "999px", // Fully rounded (pill shape) - playful, inviting
  
  // Semantic radius styles
  styles: {
    sharp: {
      value: "0px",
      description: "Conveys precision and professionalism, suited for corporate designs"
    },
    balanced: {
      value: "8px",
      description: "Modern approach blending formality with softness, versatile for tech products"
    },
    friendly: {
      value: "999px",
      description: "Playful and approachable character, ideal for social apps and creative products"
    }
  }
};

## Stroke 
// 5. STROKE TOKENS
const FigrStroke = {
  width: {
    fine: "1.2px", // Fine stroke - precision and subtlety
    medium: "1.5px", // Medium stroke - balanced and adaptable
    thick: "4px" // Thick stroke - strength and emphasis
  },
  style: {
    solid: "solid",
    dashed: "dashed",
    dotted: "dotted"
  },
  
  // Semantic stroke styles
  styles: {
    fine: {
      width: "1.2px",
      description: "Precision and subtlety, refined and sophisticated feel"
    },
    medium: {
      width: "1.5px",
      description: "Balanced and adaptable, ensuring clarity without overpowering"
    },
    thick: {
      width: "4px",
      description: "Strength and emphasis, makes key elements stand out"
    }
  }
};
## Spacing 
// 6. SPACING TOKENS
const FigrSpacing = {
  // Base spacing scale
  0: "0px",
  1: "4px",
  2: "8px",
  3: "12px",
  4: "16px",
  5: "20px",
  6: "24px",
  7: "28px",
  8: "32px",
  9: "36px",
  10: "40px",
  
  // Semantic spacing compositions
  layout: {
    compact: {
      spacing: "8px",
      padding: "12px",
      description: "Dense and focused layout for content-heavy interfaces"
    },
    balanced: {
      spacing: "16px",
      padding: "24px",
      description: "Comfortable layout with good readability and navigation"
    },
    expanded: {
      spacing: "32px",
      padding: "40px",
      description: "Open and elegant spacing for minimalist designs"
    }
  }
};

// Export all token categories
const FigrDesignTokens = {
  colors: FigrColors,
  typography: FigrTypography,
  effects: FigrEffects,
  radius: FigrRadius,
  stroke: FigrStroke,
  spacing: FigrSpacing
};

export default FigrDesignTokens;

// Individual exports for modular usage
export {
  FigrColors,
  FigrTypography,
  FigrEffects,
  FigrRadius,
  FigrStroke,
  FigrSpacing
};


## Installation and Usage 

## Web (CSS variable)
/**
 * SIDHE Design System - Web Implementation
 * 
 * This file demonstrates how to implement the SIDHE design tokens in a web project.
 */

/**
 * 1. Import the design tokens
 * You can import the pre-generated CSS file:
 */

/* In your HTML */
// <link rel="stylesheet" href="path/to/sidhe-tokens.css">

/* Or in your CSS/SCSS */
// @import 'node_modules/@sidhe/design-tokens/dist/web/sidhe-tokens.css';


/**
 * 2. Implementation Examples
 */

/* Button Components */
.button {
  /* Base button styles */
  display: inline-flex;
  align-items: center;
  justify-content: center;
  font-family: var(--sidhe-font-family-primary);
  font-weight: var(--sidhe-font-weight-medium);
  font-size: var(--sidhe-font-size-md);
  padding: var(--sidhe-spacing-3) var(--sidhe-spacing-6);
  border-radius: var(--sidhe-radius-base8);
  transition: background-color 0.2s, box-shadow 0.2s;
  border: none;
  cursor: pointer;
}

.button-primary {
  background-color: var(--sidhe-color-primary-500);
  color: white;
  box-shadow: var(--sidhe-effect-elevation-1);
}

.button-primary:hover {
  background-color: var(--sidhe-color-primary-400);
  box-shadow: var(--sidhe-effect-elevation-2);
}

.button-secondary {
  background-color: var(--sidhe-color-secondary-500);
  color: white;
  box-shadow: var(--sidhe-effect-elevation-1);
}

.button-secondary:hover {
  background-color: var(--sidhe-color-secondary-400);
  box-shadow: var(--sidhe-effect-elevation-2);
}

.button-ghost {
  background-color: transparent;
  color: var(--sidhe-color-neutral-900);
  box-shadow: none;
}

.button-ghost:hover {
  background-color: var(--sidhe-color-neutral-100);
}

/* Card Component */
.card {
  background-color: white;
  border-radius: var(--sidhe-radius-base8);
  box-shadow: var(--sidhe-effect-elevation-2);
  padding: var(--sidhe-spacing-6);
}

.card-header {
  margin-bottom: var(--sidhe-spacing-4);
}

.card-title {
  font-family: var(--sidhe-font-family-secondary);
  font-size: var(--sidhe-font-size-2xl);
  font-weight: var(--sidhe-font-weight-bold);
  color: var(--sidhe-color-neutral-900);
  margin: 0 0 var(--sidhe-spacing-2) 0;
}

.card-subtitle {
  font-family: var(--sidhe-font-family-primary);
  font-size: var(--sidhe-font-size-md);
  color: var(--sidhe-color-neutral-600);
  margin: 0;
}

.card-content {
  font-family: var(--sidhe-font-family-primary);
  font-size: var(--sidhe-font-size-md);
  line-height: var(--sidhe-line-height-normal);
  color: var(--sidhe-color-neutral-800);
}

/* Typography System */
.heading-1 {
  font-family: var(--sidhe-font-family-secondary);
  font-size: var(--sidhe-font-size-5xl);
  font-weight: var(--sidhe-font-weight-bold);
  line-height: var(--sidhe-line-height-tight);
  letter-spacing: var(--sidhe-letter-spacing-tight);
  color: var(--sidhe-color-neutral-900);
}

.heading-2 {
  font-family: var(--sidhe-font-family-secondary);
  font-size: var(--sidhe-font-size-4xl);
  font-weight: var(--sidhe-font-weight-bold);
  line-height: var(--sidhe-line-height-tight);
  letter-spacing: var(--sidhe-letter-spacing-tight);
  color: var(--sidhe-color-neutral-900);
}

.heading-3 {
  font-family: var(--sidhe-font-family-secondary);
  font-size: var(--sidhe-font-size-3xl);
  font-weight: var(--sidhe-font-weight-semibold);
  line-height: var(--sidhe-line-height-tight);
  color: var(--sidhe-color-neutral-900);
}

.body-text {
  font-family: var(--sidhe-font-family-primary);
  font-size: var(--sidhe-font-size-md);
  font-weight: var(--sidhe-font-weight-regular);
  line-height: var(--sidhe-line-height-normal);
  color: var(--sidhe-color-neutral-800);
}

.body-text-small {
  font-family: var(--sidhe-font-family-primary);
  font-size: var(--sidhe-font-size-sm);
  font-weight: var(--sidhe-font-weight-regular);
  line-height: var(--sidhe-line-height-normal);
  color: var(--sidhe-color-neutral-800);
}

.caption {
  font-family: var(--sidhe-font-family-primary);
  font-size: var(--sidhe-font-size-xs);
  font-weight: var(--sidhe-font-weight-regular);
  line-height: var(--sidhe-line-height-normal);
  color: var(--sidhe-color-neutral-600);
}

/* Form Components */
.input {
  font-family: var(--sidhe-font-family-primary);
  font-size: var(--sidhe-font-size-md);
  color: var(--sidhe-color-neutral-900);
  padding: var(--sidhe-spacing-3) var(--sidhe-spacing-4);
  border: 1px solid var(--sidhe-color-neutral-300);
  border-radius: var(--sidhe-radius-base4);
  background-color: white;
  transition: border-color 0.2s, box-shadow 0.2s;
  box-shadow: var(--sidhe-effect-sunken-sm);
}

.input:focus {
  outline: none;
  border-color: var(--sidhe-color-primary-500);
  box-shadow: 0 0 0 3px var(--sidhe-color-primary-10);
}

.input-label {
  display: block;
  font-family: var(--sidhe-font-family-primary);
  font-size: var(--sidhe-font-size-sm);
  font-weight: var(--sidhe-font-weight-medium);
  color: var(--sidhe-color-neutral-800);
  margin-bottom: var(--sidhe-spacing-2);
}

/* Alert Components */
.alert {
  padding: var(--sidhe-spacing-4);
  border-radius: var(--sidhe-radius-base4);
  margin-bottom: var(--sidhe-spacing-4);
  display: flex;
  align-items: flex-start;
}

.alert-info {
  background-color: var(--sidhe-color-secondary-10);
  border-left: var(--sidhe-stroke-width-medium) solid var(--sidhe-color-secondary-500);
}

.alert-success {
  background-color: var(--sidhe-color-green-10);
  border-left: var(--sidhe-stroke-width-medium) solid var(--sidhe-color-green-200);
}

.alert-warning {
  background-color: var(--sidhe-color-yellow-10);
  border-left: var(--sidhe-stroke-width-medium) solid var(--sidhe-color-yellow-200);
}

.alert-error {
  background-color: var(--sidhe-color-red-10);
  border-left: var(--sidhe-stroke-width-medium) solid var(--sidhe-color-red-200);
}

/* Layout System */
.container {
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 var(--sidhe-spacing-4);
}

.layout-stack-sm > * + * {
  margin-top: var(--sidhe-spacing-2);
}

.layout-stack-md > * + * {
  margin-top: var(--sidhe-spacing-4);
}

.layout-stack-lg > * + * {
  margin-top: var(--sidhe-spacing-8);
}

/* Example Usage in HTML
<div class="container">
  <h1 class="heading-1">SIDHE Design System</h1>
  
  <div class="card">
    <div class="card-header">
      <h2 class="card-title">Welcome</h2>
      <p class="card-subtitle">Design system implementation</p>
    </div>
    <div class="card-content">
      <p class="body-text">This is an example of the SIDHE design system implementation.</p>
    </div>
  </div>
  
  <div class="layout-stack-md">
    <div class="alert alert-info">
      <p class="body-text">This is an informational message.</p>
    </div>
    
    <form>
      <div class="layout-stack-sm">
        <label class="input-label">Full Name</label>
        <input type="text" class="input" placeholder="Enter your name">
      </div>
      
      <div class="layout-stack-sm" style="margin-top: var(--sidhe-spacing-4);">
        <button class="button button-primary">Submit</button>
        <button class="button button-ghost">Cancel</button>
      </div>
    </form>
  </div>
</div>
*/

## IOS (Swift) 

/**
 * SIDHE Design System - iOS Implementation
 * 
 * This file demonstrates how to implement the SIDHE design tokens in an iOS project using Swift.
 */

import UIKit
import SwiftUI

// MARK: - Design Tokens

/// SIDHE Design System color tokens
struct SIDHEColors {
    // Primary Colors
    struct Primary {
        static let color100 = UIColor(red: 246/255, green: 134/255, blue: 194/255, alpha: 1) // #F686C2
        static let color200 = UIColor(red: 244/255, green: 91/255, blue: 182/255, alpha: 1)  // #F45BB6
        static let color300 = UIColor(red: 242/255, green: 51/255, blue: 171/255, alpha: 1)  // #F233AB
        static let color400 = UIColor(red: 239/255, green: 10/255, blue: 159/255, alpha: 1)  // #EF0A9F
        static let color500 = UIColor(red: 236/255, green: 0/255, blue: 148/255, alpha: 1)   // #EC0094
        static let color10 = UIColor(red: 236/255, green: 0/255, blue: 148/255, alpha: 0.1)  // rgba(236, 0, 148, 0.1)
    }
    
    // Secondary Colors
    struct Secondary {
        static let color100 = UIColor(red: 168/255, green: 136/255, blue: 229/255, alpha: 1) // #A888E5
        static let color200 = UIColor(red: 140/255, green: 89/255, blue: 221/255, alpha: 1)  // #8C59DD
        static let color300 = UIColor(red: 112/255, green: 43/255, blue: 213/255, alpha: 1)  // #702BD5
        static let color400 = UIColor(red: 85/255, green: 0/255, blue: 204/255, alpha: 1)    // #5500CC
        static let color500 = UIColor(red: 58/255, green: 0/255, blue: 153/255, alpha: 1)    // #3A0099
        static let color10 = UIColor(red: 58/255, green: 0/255, blue: 153/255, alpha: 0.1)   // rgba(58, 0, 153, 0.1)
    }
    
    // Neutral Colors
    struct Neutral {
        static let color100 = UIColor(red: 245/255, green: 245/255, blue: 245/255, alpha: 1) // #F5F5F5
        static let color200 = UIColor(red: 224/255, green: 224/255, blue: 224/255, alpha: 1) // #E0E0E0
        static let color300 = UIColor(red: 189/255, green: 189/255, blue: 189/255, alpha: 1) // #BDBDBD
        static let color400 = UIColor(red: 158/255, green: 158/255, blue: 158/255, alpha: 1) // #9E9E9E
        static let color500 = UIColor(red: 117/255, green: 117/255, blue: 117/255, alpha: 1) // #757575
        static let color600 = UIColor(red: 97/255, green: 97/255, blue: 97/255, alpha: 1)    // #616161
        static let color700 = UIColor(red: 66/255, green: 66/255, blue: 66/255, alpha: 1)    // #424242
        static let color800 = UIColor(red: 48/255, green: 48/255, blue: 48/255, alpha: 1)    // #303030
        static let color900 = UIColor(red: 33/255, green: 33/255, blue: 33/255, alpha: 1)    // #212121
        static let color1000 = UIColor(red: 18/255, green: 18/255, blue: 18/255, alpha: 1)   // #121212
        static let color10 = UIColor(red: 33/255, green: 33/255, blue: 33/255, alpha: 0.1)   // rgba(33, 33, 33, 0.1)
    }
    
    // Feedback Colors
    struct Red {
        static let color100 = UIColor(red: 255/255, green: 90/255, blue: 90/255, alpha: 1)   // #FF5A5A
        static let color200 = UIColor(red: 221/255, green: 14/255, blue: 16/255, alpha: 1)   // #DD0E10
        static let color10 = UIColor(red: 221/255, green: 14/255, blue: 16/255, alpha: 0.1)  // rgba(221, 14, 16, 0.1)
    }
    
    struct Yellow {
        static let color100 = UIColor(red: 255/255, green: 222/255, blue: 89/255, alpha: 1)  // #FFDE59
        static let color200 = UIColor(red: 201/255, green: 171/255, blue: 25/255, alpha: 1)  // #C9AB19
        static let color10 = UIColor(red: 201/255, green: 171/255, blue: 25/255, alpha: 0.1) // rgba(201, 171, 25, 0.1)
    }
    
    struct Green {
        static let color100 = UIColor(red: 86/255, green: 224/255, blue: 178/255, alpha: 1)  // #56E0B2
        static let color200 = UIColor(red: 23/255, green: 175/255, blue: 102/255, alpha: 1)  // #17AF66
        static let color10 = UIColor(red: 23/255, green: 175/255, blue: 102/255, alpha: 0.1) // rgba(23, 175, 102, 0.1)
    }
}

/// SIDHE Design System typography tokens
struct SIDHETypography {
    // Font Families
    struct FontFamily {
        static let primary = "PlusJakartaSans-Regular" // Use appropriate font names registered in the app
        static let primaryMedium = "PlusJakartaSans-Medium"
        static let primarySemiBold = "PlusJakartaSans-SemiBold"
        static let primaryBold = "PlusJakartaSans-Bold"
        
        static let secondary = "Lora-Regular"
        static let secondaryMedium = "Lora-Medium"
        static let secondarySemiBold = "Lora-SemiBold"
        static let secondaryBold = "Lora-Bold"
    }
    
    // Font Weights
    struct FontWeight {
        static let regular = UIFont.Weight.regular
        static let medium = UIFont.Weight.medium
        static let semiBold = UIFont.Weight.semibold
        static let bold = UIFont.Weight.bold
    }
    
    // Font Sizes
    struct FontSize {
        static let xs: CGFloat = 12
        static let sm: CGFloat = 14
        static let md: CGFloat = 16
        static let lg: CGFloat = 18
        static let xl: CGFloat = 20
        static let xxl: CGFloat = 24
        static let xxxl: CGFloat = 30
        static let xxxxl: CGFloat = 36
        static let xxxxxl: CGFloat = 48
        static let xxxxxxl: CGFloat = 60
    }
    
    // Line Heights
    struct LineHeight {
        static let none: CGFloat = 1.0
        static let tight: CGFloat = 1.25
        static let snug: CGFloat = 1.375
        static let normal: CGFloat = 1.5
        static let relaxed: CGFloat = 1.625
        static let loose: CGFloat = 2.0
    }
}

/// SIDHE Design System spacing tokens
struct SIDHESpacing {
    static let spacing0: CGFloat = 0
    static let spacing1: CGFloat = 4
    static let spacing2: CGFloat = 8
    static let spacing3: CGFloat = 12
    static let spacing4: CGFloat = 16
    static let spacing5: CGFloat = 20
    static let spacing6: CGFloat = 24
    static let spacing8: CGFloat = 32
    static let spacing10: CGFloat = 40
}

/// SIDHE Design System radius tokens
struct SIDHERadius {
    static let base0: CGFloat = 0
    static let base2: CGFloat = 2
    static let base4: CGFloat = 4
    static let base8: CGFloat = 8
    static let base12: CGFloat = 12
    static let baseRound: CGFloat = 999
}

/// SIDHE Design System effect tokens
struct SIDHEEffects {
    struct Shadow {
        static let elevation1: [String: Any] = [
            "color": UIColor(red: 0, green: 0, blue: 0, alpha: 0.1),
            "offset": CGSize(width: 0, height: 1),
            "radius": 3,
            "opacity": 0.1
        ]
        
        static let elevation2: [String: Any] = [
            "color": UIColor(red: 0, green: 0, blue: 0, alpha: 0.1),
            "offset": CGSize(width: 0, height: 3),
            "radius": 6,
            "opacity": 0.1
        ]
        
        static let elevation3: [String: Any] = [
            "color": UIColor(red: 0, green: 0, blue: 0, alpha: 0.1),
            "offset": CGSize(width: 0, height: 6),
            "radius": 12,
            "opacity": 0.1
        ]
    }
}

// MARK: - UIKit Component Extensions

// Button Component Styles
extension UIButton {
    func applySIDHEPrimaryStyle() {
        backgroundColor = SIDHEColors.Primary.color500
        setTitleColor(.white, for: .normal)
        titleLabel?.font = UIFont(name: SIDHETypography.FontFamily.primaryMedium, size: SIDHETypography.FontSize.md)
        layer.cornerRadius = SIDHERadius.base8
        contentEdgeInsets = UIEdgeInsets(
            top: SIDHESpacing.spacing3,
            left: SIDHESpacing.spacing6,
            bottom: SIDHESpacing.spacing3,
            right: SIDHESpacing.spacing6
        )
        
        // Add shadow
        layer.shadowColor = SIDHEEffects.Shadow.elevation1["color"] as? CGColor
        layer.shadowOffset = SIDHEEffects.Shadow.elevation1["offset"] as! CGSize
        layer.shadowRadius = SIDHEEffects.Shadow.elevation1["radius"] as! CGFloat
        layer.shadowOpacity = Float(SIDHEEffects.Shadow.elevation1["opacity"] as! CGFloat)
    }
    
    func applySIDHESecondaryStyle() {
        backgroundColor = SIDHEColors.Secondary.color500
        setTitleColor(.white, for: .normal)
        titleLabel?.font = UIFont(name: SIDHETypography.FontFamily.primaryMedium, size: SIDHETypography.FontSize.md)
        layer.cornerRadius = SIDHERadius.base8
        contentEdgeInsets = UIEdgeInsets(
            top: SIDHESpacing.spacing3,
            left: SIDHESpacing.spacing6,
            bottom: SIDHESpacing.spacing3,
            right: SIDHESpacing.spacing6
        )
        
        // Add shadow
        layer.shadowColor = SIDHEEffects.Shadow.elevation1["color"] as? CGColor
        layer.shadowOffset = SIDHEEffects.Shadow.elevation1["offset"] as! CGSize
        layer.shadowRadius = SIDHEEffects.Shadow.elevation1["radius"] as! CGFloat
        layer.shadowOpacity = Float(SIDHEEffects.Shadow.elevation1["opacity"] as! CGFloat)
    }
    
    func applySIDHEGhostStyle() {
        backgroundColor = .clear
        setTitleColor(SIDHEColors.Neutral.color900, for: .normal)
        titleLabel?.font = UIFont(name: SIDHETypography.FontFamily.primaryMedium, size: SIDHETypography.FontSize.md)
        layer.cornerRadius = SIDHERadius.base8
        contentEdgeInsets = UIEdgeInsets(
            top: SIDHESpacing.spacing3,
            left: SIDHESpacing.spacing6,
            bottom: SIDHESpacing.spacing3,
            right: SIDHESpacing.spacing6
        )
        layer.shadowOpacity = 0
    }
}

// Text Style Extensions
extension UILabel {
    func applySIDHEHeading1Style() {
        font = UIFont(name: SIDHETypography.FontFamily.secondaryBold, size: SIDHETypography.FontSize.xxxxxl)
        textColor = SIDHEColors.Neutral.color900
        numberOfLines = 0
        adjustsFontSizeToFitWidth = false
    }
    
    func applySIDHEHeading2Style() {
        font = UIFont(name: SIDHETypography.FontFamily.secondaryBold, size: SIDHETypography.FontSize.xxxxl)
        textColor = SIDHEColors.Neutral.color900
        numberOfLines = 0
    }
    
    func applySIDHEHeading3Style() {
        font = UIFont(name: SIDHETypography.FontFamily.secondarySemiBold, size: SIDHETypography.FontSize.xxxl)
        textColor = SIDHEColors.Neutral.color900
        numberOfLines = 0
    }
    
    func applySIDHEBodyStyle() {
        font = UIFont(name: SIDHETypography.FontFamily.primary, size: SIDHETypography.FontSize.md)
        textColor = SIDHEColors.Neutral.color800
        numberOfLines = 0
    }
    
    func applySIDHEBodySmallStyle() {
        font = UIFont(name: SIDHETypography.FontFamily.primary, size: SIDHETypography.FontSize.sm)
        textColor = SIDHEColors.Neutral.color800
        numberOfLines = 0
    }
    
    func applySIDHECaptionStyle() {
        font = UIFont(name: SIDHETypography.FontFamily.primary, size: SIDHETypography.FontSize.xs)
        textColor = SIDHEColors.Neutral.color600
        numberOfLines = 0
    }
}

// Card View Extension
extension UIView {
    func applySIDHECardStyle() {
        backgroundColor = .white
        layer.cornerRadius = SIDHERadius.base8
        
        // Add shadow
        layer.shadowColor = SIDHEEffects.Shadow.elevation2["color"] as? CGColor
        layer.shadowOffset = SIDHEEffects.Shadow.elevation2["offset"] as! CGSize
        layer.shadowRadius = SIDHEEffects.Shadow.elevation2["radius"] as! CGFloat
        layer.shadowOpacity = Float(SIDHEEffects.Shadow.elevation2["opacity"] as! CGFloat)
    }
}

// Text Field Extension
extension UITextField {
    func applySIDHEInputStyle() {
        font = UIFont(name: SIDHETypography.FontFamily.primary, size: SIDHETypography.FontSize.md)
        textColor = SIDHEColors.Neutral.color900
        
        let paddingView = UIView(frame: CGRect(x: 0, y: 0, width: SIDHESpacing.spacing4, height: 0))
        leftView = paddingView
        leftViewMode = .always
        
        layer.borderWidth = 1
        layer.borderColor = SIDHEColors.Neutral.color300.cgColor
        layer.cornerRadius = SIDHERadius.base4
        
        backgroundColor = .white
        
        // Add shadow
        layer.shadowColor = SIDHEEffects.Shadow.elevation1["color"] as? CGColor
        layer.shadowOffset = SIDHEEffects.Shadow.elevation1["offset"] as! CGSize
        layer.shadowRadius = SIDHEEffects.Shadow.elevation1["radius"] as! CGFloat
        layer.shadowOpacity = Float(SIDHEEffects.Shadow.elevation1["opacity"] as! CGFloat)
    }
}

// MARK: - SwiftUI Implementation

extension Color {
    // Primary Colors
    static let sidheP100 = Color(SIDHEColors.Primary.color100)
    static let sidheP200 = Color(SIDHEColors.Primary.color200)
    static let sidheP300 = Color(SIDHEColors.Primary.color300)
    static let sidheP400 = Color(SIDHEColors.Primary.color400)
    static let sidheP500 = Color(SIDHEColors.Primary.color500)
    
    // Secondary Colors
    static let sidheS100 = Color(SIDHEColors.Secondary.color100)
    static let sidheS200 = Color(SIDHEColors.Secondary.color200)
    static let sidheS300 = Color(SIDHEColors.Secondary.color300)
    static let sidheS400 = Color(SIDHEColors.Secondary.color400)
    static let sidheS500 = Color(SIDHEColors.Secondary.color500)
    
    // Neutral Colors
    static let sidheN100 = Color(SIDHEColors.Neutral.color100)
    static let sidheN200 = Color(SIDHEColors.Neutral.color200)
    static let sidheN300 = Color(SIDHEColors.Neutral.color300)
    static let sidheN400 = Color(SIDHEColors.Neutral.color400)
    static let sidheN500 = Color(SIDHEColors.Neutral.color500)
    static let sidheN600 = Color(SIDHEColors.Neutral.color600)
    static let sidheN700 = Color(SIDHEColors.Neutral.color700)
    static let sidheN800 = Color(SIDHEColors.Neutral.color800)
    static let sidheN900 = Color(SIDHEColors.Neutral.color900)
}

// SwiftUI Text Styles
struct SIDHETextStyles {
    struct Heading1: ViewModifier {
        func body(content: Content) -> some View {
            content
                .font(.custom(SIDHETypography.FontFamily.secondaryBold, size: SIDHETypography.FontSize.xxxxxl))
                .foregroundColor(Color(SIDHEColors.Neutral.color900))
                .lineSpacing(SIDHETypography.FontSize.xxxxxl * (SIDHETypography.LineHeight.tight - 1))
        }
    }
    
    struct Heading2: ViewModifier {
        func body(content: Content) -> some View {
            content
                .font(.custom(SIDHETypography.FontFamily.secondaryBold, size: SIDHETypography.FontSize.xxxxl))
                .foregroundColor(Color(SIDHEColors.Neutral.color900))
                .lineSpacing(SIDHETypography.FontSize.xxxxl * (SIDHETypography.LineHeight.tight - 1))
        }
    }
    
    struct Heading3: ViewModifier {
        func body(content: Content) -> some View {
            content
                .font(.custom(SIDHETypography.FontFamily.secondarySemiBold, size: SIDHETypography.FontSize.xxxl))
                .foregroundColor(Color(SIDHEColors.Neutral.color900))
                .lineSpacing(SIDHETypography.FontSize.xxxl * (SIDHETypography.LineHeight.tight - 1))
        }
    }
    
    struct BodyText: ViewModifier {
        func body(content: Content) -> some View {
            content
                .font(.custom(SIDHETypography.FontFamily.primary, size: SIDHETypography.FontSize.md))
                .foregroundColor(Color(SIDHEColors.Neutral.color800))
                .lineSpacing(SIDHETypography.FontSize.md * (SIDHETypography.LineHeight.normal - 1))
        }
    }
    
    struct BodySmall: ViewModifier {
        func body(content: Content) -> some View {
            content
                .font(.custom(SIDHETypography.FontFamily.primary, size: SIDHETypography.FontSize.sm))
                .foregroundColor(Color(SIDHEColors.Neutral.color800))
                .lineSpacing(SIDHETypography.FontSize.sm * (SIDHETypography.LineHeight.normal - 1))
        }
    }
    
    struct Caption: ViewModifier {
        func body(content: Content) -> some View {
            content
                .font(.custom(SIDHETypography.FontFamily.primary, size: SIDHETypography.FontSize.xs))
                .foregroundColor(Color(SIDHEColors.Neutral.color600))
                .lineSpacing(SIDHETypography.FontSize.xs * (SIDHETypography.LineHeight.normal - 1))
        }
    }
}

extension View {
    func sidheHeading1() -> some View {
        modifier(SIDHETextStyles.Heading1())
    }
    
    func sidheHeading2() -> some View {
        modifier(SIDHETextStyles.Heading2())
    }
    
    func sidheHeading3() -> some View {
        modifier(SIDHETextStyles.Heading3())
    }
    
    func sidheBodyText() -> some View {
        modifier(SIDHETextStyles.BodyText())
    }
    
    func sidheBodySmall() -> some View {
        modifier(SIDHETextStyles.BodySmall())
    }
    
    func sidheCaption() -> some View {
        modifier(SIDHETextStyles.Caption())
    }
}

// SwiftUI Button Styles
struct SIDHEPrimaryButtonStyle: ButtonStyle {
    func makeBody(configuration: Configuration) -> some View {
        configuration.label
            .padding(.vertical, SIDHESpacing.spacing3)
            .padding(.horizontal, SIDHESpacing.spacing6)
            .background(
                configuration.isPressed ? Color(SIDHEColors.Primary.color400) : Color(SIDHEColors.Primary.color500)
            )
            .foregroundColor(.white)
            .cornerRadius(SIDHERadius.base8)
            .font(.custom(SIDHETypography.FontFamily.primaryMedium, size: SIDHETypography.FontSize.md))
            .shadow(
                color: Color(SIDHEColors.Neutral.color900).opacity(0.1),
                radius: 3,
                x: 0,
                y: 1
            )
    }
}

struct SIDHESecondaryButtonStyle: ButtonStyle {
    func makeBody(configuration: Configuration) -> some View {
        configuration.label
            .padding(.vertical, SIDHESpacing.spacing3)
            .padding(.horizontal, SIDHESpacing.spacing6)
            .background(
                configuration.isPressed ? Color(SIDHEColors.Secondary.color400) : Color(SIDHEColors.Secondary.color500)
            )
            .foregroundColor(.white)
            .cornerRadius(SIDHERadius.base8)
            .font(.custom(SIDHETypography.FontFamily.primaryMedium, size: SIDHETypography.FontSize.md))
            .shadow(
                color: Color(SIDHEColors.Neutral.color900).opacity(0.1),
                radius: 3,
                x: 0,
                y: 1
            )
    }
}

struct SIDHEGhostButtonStyle: ButtonStyle {
    func makeBody(configuration: Configuration) -> some View {
        configuration.label
            .padding(.vertical, SIDHESpacing.spacing3)
            .padding(.horizontal, SIDHESpacing.spacing6)
            .background(
                configuration.isPressed ? Color(SIDHEColors.Neutral.color100) : Color.clear
            )
            .foregroundColor(Color(SIDHEColors.Neutral.color900))
            .cornerRadius(SIDHERadius.base8)
            .font(.custom(SIDHETypography.FontFamily.primaryMedium, size: SIDHETypography.FontSize.md))
    }
}

// SwiftUI Card View
struct SIDHECard<Content: View>: View {
    let content: Content
    
    init(@ViewBuilder content: () -> Content) {
        self.content = content()
    }
    
    var body: some View {
        content
            .padding(SIDHESpacing.spacing6)
            .background(Color.white)
            .cornerRadius(SIDHERadius.base8)
            .shadow(
                color: Color(SIDHEColors.Neutral.color900).opacity(0.1),
                radius: 6,
                x: 0,
                y: 3
            )
    }
}

// Example Usage with SwiftUI:
/*
struct ContentView: View {
    @State private var name = ""
    
    var body: some View {
        VStack(alignment: .leading, spacing: SIDHESpacing.spacing6) {
            Text("SIDHE Design System")
                .sidheHeading1()
            
            SIDHECard {
                VStack(alignment: .leading, spacing: SIDHESpacing.spacing4) {
                    Text("Welcome")
                        .sidheHeading2()
                    
                    Text("Design system implementation")
                        .sidheBodySmall()
                    
                    Text("This is an example of the SIDHE design system implementation.")
                        .sidheBodyText()
                        .padding(.top, SIDHESpacing.spacing2)
                }
            }
            
            VStack(alignment: .leading, spacing: SIDHESpacing.spacing4) {
                Text("Your Information")
                    .sidheHeading3()
                
                VStack(alignment: .leading, spacing: SIDHESpacing.spacing2) {
                    Text("Full Name")
                        .sidheCaption()
                    
                    TextField("Enter your name", text: $name)
                        .padding(.vertical, SIDHESpacing.spacing3)
                        .padding(.horizontal, SIDHESpacing.spacing4)
                        .background(Color.white)
                        .cornerRadius(SIDHERadius.base4)
                        .overlay(
                            RoundedRectangle(cornerRadius: SIDHERadius.base4)
                                .stroke(Color(SIDHEColors.Neutral.color300), lineWidth: 1)
                        )
                }
                
                HStack(spacing: SIDHESpacing.spacing4) {
                    Button("Submit") {
                        // Action
                    }
                    .buttonStyle(SIDHEPrimaryButtonStyle())
                    
                    Button("Cancel") {
                        // Action
                    }
                    .buttonStyle(SIDHEGhostButtonStyle())
                }
                .padding(.top, SIDHESpacing.spacing4)
            }
            
            Spacer()
        }
        .padding(SIDHESpacing.spacing6)
    }
}
*/

## Android (XML) 
<!-- 
  SIDHE Design System - Android Implementation Guide
  
  This file demonstrates how to implement the SIDHE design tokens in an Android project using XML resources.
  The implementation is separated into multiple resource files following Android best practices.
-->

<!-- res/values/sidhe_colors.xml -->
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <!-- Primary Colors -->
    <color name="sidhe_color_primary_100">#FFF686C2</color>
    <color name="sidhe_color_primary_200">#FFF45BB6</color>
    <color name="sidhe_color_primary_300">#FFF233AB</color>
    <color name="sidhe_color_primary_400">#FFEF0A9F</color>
    <color name="sidhe_color_primary_500">#FFEC0094</color>
    <color name="sidhe_color_primary_10">#1AEC0094</color>

    <!-- Secondary Colors -->
    <color name="sidhe_color_secondary_100">#FFA888E5</color>
    <color name="sidhe_color_secondary_200">#FF8C59DD</color>
    <color name="sidhe_color_secondary_300">#FF702BD5</color>
    <color name="sidhe_color_secondary_400">#FF5500CC</color>
    <color name="sidhe_color_secondary_500">#FF3A0099</color>
    <color name="sidhe_color_secondary_10">#1A3A0099</color>

    <!-- Neutral Colors -->
    <color name="sidhe_color_neutral_100">#FFF5F5F5</color>
    <color name="sidhe_color_neutral_200">#FFE0E0E0</color>
    <color name="sidhe_color_neutral_300">#FFBDBDBD</color>
    <color name="sidhe_color_neutral_400">#FF9E9E9E</color>
    <color name="sidhe_color_neutral_500">#FF757575</color>
    <color name="sidhe_color_neutral_600">#FF616161</color>
    <color name="sidhe_color_neutral_700">#FF424242</color>
    <color name="sidhe_color_neutral_800">#FF303030</color>
    <color name="sidhe_color_neutral_900">#FF212121</color>
    <color name="sidhe_color_neutral_1000">#FF121212</color>
    <color name="sidhe_color_neutral_10">#1A212121</color>

    <!-- Feedback Colors -->
    <color name="sidhe_color_red_100">#FFFF5A5A</color>
    <color name="sidhe_color_red_200">#FFDD0E10</color>
    <color name="sidhe_color_red_10">#1ADD0E10</color>

    <color name="sidhe_color_yellow_100">#FFFFDE59</color>
    <color name="sidhe_color_yellow_200">#FFC9AB19</color>
    <color name="sidhe_color_yellow_10">#1AC9AB19</color>

    <color name="sidhe_color_green_100">#FF56E0B2</color>
    <color name="sidhe_color_green_200">#FF17AF66</color>
    <color name="sidhe_color_green_10">#1A17AF66</color>
</resources>

<!-- res/values/sidhe_dimens.xml -->
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <!-- Spacing Tokens -->
    <dimen name="sidhe_spacing_0">0dp</dimen>
    <dimen name="sidhe_spacing_1">4dp</dimen>
    <dimen name="sidhe_spacing_2">8dp</dimen>
    <dimen name="sidhe_spacing_3">12dp</dimen>
    <dimen name="sidhe_spacing_4">16dp</dimen>
    <dimen name="sidhe_spacing_5">20dp</dimen>
    <dimen name="sidhe_spacing_6">24dp</dimen>
    <dimen name="sidhe_spacing_7">28dp</dimen>
    <dimen name="sidhe_spacing_8">32dp</dimen>
    <dimen name="sidhe_spacing_9">36dp</dimen>
    <dimen name="sidhe_spacing_10">40dp</dimen>

    <!-- Radius Tokens -->
    <dimen name="sidhe_radius_0">0dp</dimen>
    <dimen name="sidhe_radius_2">2dp</dimen>
    <dimen name="sidhe_radius_4">4dp</dimen>
    <dimen name="sidhe_radius_8">8dp</dimen>
    <dimen name="sidhe_radius_12">12dp</dimen>
    <item name="sidhe_radius_round" format="float" type="dimen">999dp</item>

    <!-- Stroke Tokens -->
    <dimen name="sidhe_stroke_width_fine">1.2dp</dimen>
    <dimen name="sidhe_stroke_width_medium">1.5dp</dimen>
    <dimen name="sidhe_stroke_width_thick">4dp</dimen>

    <!-- Typography - Font Sizes -->
    <dimen name="sidhe_font_size_xs">12sp</dimen>
    <dimen name="sidhe_font_size_sm">14sp</dimen>
    <dimen name="sidhe_font_size_md">16sp</dimen>
    <dimen name="sidhe_font_size_lg">18sp</dimen>
    <dimen name="sidhe_font_size_xl">20sp</dimen>
    <dimen name="sidhe_font_size_2xl">24sp</dimen>
    <dimen name="sidhe_font_size_3xl">30sp</dimen>
    <dimen name="sidhe_font_size_4xl">36sp</dimen>
    <dimen name="sidhe_font_size_5xl">48sp</dimen>
    <dimen name="sidhe_font_size_6xl">60sp</dimen>

    <!-- Line Heights (as multipliers) -->
    <item name="sidhe_line_height_none" format="float" type="dimen">1.0</item>
    <item name="sidhe_line_height_tight" format="float" type="dimen">1.25</item>
    <item name="sidhe_line_height_snug" format="float" type="dimen">1.375</item>
    <item name="sidhe_line_height_normal" format="float" type="dimen">1.5</item>
    <item name="sidhe_line_height_relaxed" format="float" type="dimen">1.625</item>
    <item name="sidhe_line_height_loose" format="float" type="dimen">2.0</item>

    <!-- Elevation Values -->
    <dimen name="sidhe_elevation_0">0dp</dimen>
    <dimen name="sidhe_elevation_1">2dp</dimen>
    <dimen name="sidhe_elevation_2">4dp</dimen>
    <dimen name="sidhe_elevation_3">8dp</dimen>
</resources>

<!-- res/values/sidhe_typography.xml -->
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <!-- Font Families -->
    <string name="sidhe_font_family_primary">sans-serif</string>
    <string name="sidhe_font_family_secondary">serif</string>
    <!-- Note: For custom fonts, you would add them to the assets/fonts folder
         and reference them in your styles using fontFamily attribute -->

    <!-- Typography Styles -->
    <!-- Heading Styles -->
    <style name="Sidhe.TextAppearance.Heading1" parent="TextAppearance.MaterialComponents.Headline1">
        <item name="fontFamily">@string/sidhe_font_family_secondary</item>
        <item name="android:fontFamily">@string/sidhe_font_family_secondary</item>
        <item name="android:textSize">@dimen/sidhe_font_size_5xl</item>
        <item name="android:textColor">@color/sidhe_color_neutral_900</item>
        <item name="android:textStyle">bold</item>
        <item name="lineHeight">@dimen/sidhe_line_height_tight</item>
        <item name="android:letterSpacing">-0.02</item>
    </style>

    <style name="Sidhe.TextAppearance.Heading2" parent="TextAppearance.MaterialComponents.Headline2">
        <item name="fontFamily">@string/sidhe_font_family_secondary</item>
        <item name="android:fontFamily">@string/sidhe_font_family_secondary</item>
        <item name="android:textSize">@dimen/sidhe_font_size_4xl</item>
        <item name="android:textColor">@color/sidhe_color_neutral_900</item>
        <item name="android:textStyle">bold</item>
        <item name="lineHeight">@dimen/sidhe_line_height_tight</item>
        <item name="android:letterSpacing">-0.02</item>
    </style>

    <style name="Sidhe.TextAppearance.Heading3" parent="TextAppearance.MaterialComponents.Headline3">
        <item name="fontFamily">@string/sidhe_font_family_secondary</item>
        <item name="android:fontFamily">@string/sidhe_font_family_secondary</item>
        <item name="android:textSize">@dimen/sidhe_font_size_3xl</item>
        <item name="android:textColor">@color/sidhe_color_neutral_900</item>
        <item name="android:textStyle">bold</item>
        <item name="lineHeight">@dimen/sidhe_line_height_tight</item>
    </style>

    <!-- Body Styles -->
    <style name="Sidhe.TextAppearance.Body" parent="TextAppearance.MaterialComponents.Body1">
        <item name="fontFamily">@string/sidhe_font_family_primary</item>
        <item name="android:fontFamily">@string/sidhe_font_family_primary</item>
        <item name="android:textSize">@dimen/sidhe_font_size_md</item>
        <item name="android:textColor">@color/sidhe_color_neutral_800</item>
        <item name="lineHeight">@dimen/sidhe_line_height_normal</item>
    </style>

    <style name="Sidhe.TextAppearance.BodySmall" parent="TextAppearance.MaterialComponents.Body2">
        <item name="fontFamily">@string/sidhe_font_family_primary</item>
        <item name="android:fontFamily">@string/sidhe_font_family_primary</item>
        <item name="android:textSize">@dimen/sidhe_font_size_sm</item>
        <item name="android:textColor">@color/sidhe_color_neutral_800</item>
        <item name="lineHeight">@dimen/sidhe_line_height_normal</item>
    </style>

    <style name="Sidhe.TextAppearance.Caption" parent="TextAppearance.MaterialComponents.Caption">
        <item name="fontFamily">@string/sidhe_font_family_primary</item>
        <item name="android:fontFamily">@string/sidhe_font_family_primary</item>
        <item name="android:textSize">@dimen/sidhe_font_size_xs</item>
        <item name="android:textColor">@color/sidhe_color_neutral_600</item>
        <item name="lineHeight">@dimen/sidhe_line_height_normal</item>
    </style>
</resources>

<!-- res/values/sidhe_styles.xml -->
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <!-- Button Styles -->
    <style name="Sidhe.Button" parent="Widget.MaterialComponents.Button">
        <item name="android:letterSpacing">0</item>
        <item name="android:textAllCaps">false</item>
        <item name="cornerRadius">@dimen/sidhe_radius_8</item>
        <item name="android:paddingTop">@dimen/sidhe_spacing_3</item>
        <item name="android:paddingBottom">@dimen/sidhe_spacing_3</item>
        <item name="android:paddingStart">@dimen/sidhe_spacing_6</item>
        <item name="android:paddingEnd">@dimen/sidhe_spacing_6</item>
    </style>

    <style name="Sidhe.Button.Primary">
        <item name="backgroundTint">@color/sidhe_color_primary_500</item>
        <item name="android:textColor">@android:color/white</item>
        <item name="android:textSize">@dimen/sidhe_font_size_md</item>
        <item name="elevation">@dimen/sidhe_elevation_1</item>
    </style>

    <style name="Sidhe.Button.Secondary">
        <item name="backgroundTint">@color/sidhe_color_secondary_500</item>
        <item name="android:textColor">@android:color/white</item>
        <item name="android:textSize">@dimen/sidhe_font_size_md</item>
        <item name="elevation">@dimen/sidhe_elevation_1</item>
    </style>

    <style name="Sidhe.Button.Ghost" parent="Widget.MaterialComponents.Button.TextButton">
        <item name="android:textColor">@color/sidhe_color_neutral_900</item>
        <item name="android:textSize">@dimen/sidhe_font_size_md</item>
        <item name="rippleColor">@color/sidhe_color_neutral_200</item>
        <item name="cornerRadius">@dimen/sidhe_radius_8</item>
        <item name="android:paddingTop">@dimen/sidhe_spacing_3</item>
        <item name="android:paddingBottom">@dimen/sidhe_spacing_3</item>
        <item name="android:paddingStart">@dimen/sidhe_spacing_6</item>
        <item name="android:paddingEnd">@dimen/sidhe_spacing_6</item>
    </style>

    <!-- Card Styles -->
    <style name="Sidhe.Card" parent="Widget.MaterialComponents.CardView">
        <item name="cardCornerRadius">@dimen/sidhe_radius_8</item>
        <item name="cardElevation">@dimen/sidhe_elevation_2</item>
        <item name="contentPadding">@dimen/sidhe_spacing_6</item>
        <item name="cardBackgroundColor">@android:color/white</item>
    </style>

    <!-- Text Input Styles -->
    <style name="Sidhe.TextInputLayout" parent="Widget.MaterialComponents.TextInputLayout.OutlinedBox">
        <item name="boxCornerRadiusBottomEnd">@dimen/sidhe_radius_4</item>
        <item name="boxCornerRadiusBottomStart">@dimen/sidhe_radius_4</item>
        <item name="boxCornerRadiusTopEnd">@dimen/sidhe_radius_4</item>
        <item name="boxCornerRadiusTopStart">@dimen/sidhe_radius_4</item>
        <item name="boxStrokeColor">@color/sidhe_color_neutral_300</item>
        <item name="hintTextColor">@color/sidhe_color_neutral_600</item>
    </style>

    <style name="Sidhe.TextInputLayout.Active">
        <item name="boxStrokeColor">@color/sidhe_color_primary_500</item>
        <item name="hintTextColor">@color/sidhe_color_primary_500</item>
    </style>

    <style name="Sidhe.TextInputEditText" parent="Widget.MaterialComponents.TextInputEditText.OutlinedBox">
        <item name="android:textAppearance">@style/Sidhe.TextAppearance.Body</item>
        <item name="android:paddingTop">@dimen/sidhe_spacing_3</item>
        <item name="android:paddingBottom">@dimen/sidhe_spacing_3</item>
    </style>

    <!-- Alert Styles -->
    <style name="Sidhe.Alert" parent="">
        <item name="android:padding">@dimen/sidhe_spacing_4</item>
        <item name="cornerRadius">@dimen/sidhe_radius_4</item>
        <item name="android:layout_marginBottom">@dimen/sidhe_spacing_4</item>
    </style>

    <style name="Sidhe.Alert.Info">
        <item name="android:background">@color/sidhe_color_secondary_10</item>
        <item name="sidhe_border_start_color">@color/sidhe_color_secondary_500</item>
    </style>

    <style name="Sidhe.Alert.Success">
        <item name="android:background">@color/sidhe_color_green_10</item>
        <item name="sidhe_border_start_color">@color/sidhe_color_green_200</item>
    </style>

    <style name="Sidhe.Alert.Warning">
        <item name="android:background">@color/sidhe_color_yellow_10</item>
        <item name="sidhe_border_start_color">@color/sidhe_color_yellow_200</item>
    </style>

    <style name="Sidhe.Alert.Error">
        <item name="android:background">@color/sidhe_color_red_10</item>
        <item name="sidhe_border_start_color">@color/sidhe_color_red_200</item>
    </style>
</resources>

<!-- res/values/themes.xml -->
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <!-- Base application theme -->
    <style name="Theme.Sidhe" parent="Theme.MaterialComponents.Light.NoActionBar">
        <!-- Primary brand color -->
        <item name="colorPrimary">@color/sidhe_color_primary_500</item>
        <item name="colorPrimaryVariant">@color/sidhe_color_primary_400</item>
        <item name="colorOnPrimary">@android:color/white</item>
        
        <!-- Secondary brand color -->
        <item name="colorSecondary">@color/sidhe_color_secondary_500</item>
        <item name="colorSecondaryVariant">@color/sidhe_color_secondary_400</item>
        <item name="colorOnSecondary">@android:color/white</item>
        
        <!-- Status bar color -->
        <item name="android:statusBarColor">?attr/colorPrimaryVariant</item>
        
        <!-- Default typography -->
        <item name="android:textViewStyle">@style/Sidhe.TextAppearance.Body</item>
        <item name="textAppearanceHeadline1">@style/Sidhe.TextAppearance.Heading1</item>
        <item name="textAppearanceHeadline2">@style/Sidhe.TextAppearance.Heading2</item>
        <item name="textAppearanceHeadline3">@style/Sidhe.TextAppearance.Heading3</item>
        <item name="textAppearanceBody1">@style/Sidhe.TextAppearance.Body</item>
        <item name="textAppearanceBody2">@style/Sidhe.TextAppearance.BodySmall</item>
        <item name="textAppearanceCaption">@style/Sidhe.TextAppearance.Caption</item>
        
        <!-- Button styles -->
        <item name="materialButtonStyle">@style/Sidhe.Button.Primary</item>
        <item name="borderlessButtonStyle">@style/Sidhe.Button.Ghost</item>
        
        <!-- Card styles -->
        <item name="materialCardViewStyle">@style/Sidhe.Card</item>
        
        <!-- Text Input styles -->
        <item name="textInputStyle">@style/Sidhe.TextInputLayout</item>
    </style>
</resources>

<!-- Example layout: res/layout/sidhe_component_examples.xml -->
<?xml version="1.0" encoding="utf-8"?>
<androidx.core.widget.NestedScrollView
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@color/sidhe_color_neutral_100">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        android:padding="@dimen/sidhe_spacing_6">

        <!-- Headings Example -->
        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="SIDHE Design System"
            android:textAppearance="@style/Sidhe.TextAppearance.Heading1"/>

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="Component Examples"
            android:textAppearance="@style/Sidhe.TextAppearance.Heading2"
            android:layout_marginTop="@dimen/sidhe_spacing_4"/>

        <!-- Card Example -->
        <com.google.android.material.card.MaterialCardView
            style="@style/Sidhe.Card"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="@dimen/sidhe_spacing_6">

            <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:orientation="vertical">

                <TextView
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:text="Welcome"
                    android:textAppearance="@style/Sidhe.TextAppearance.Heading3"/>

                <TextView
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:text="Design system implementation"
                    android:textAppearance="@style/Sidhe.TextAppearance.BodySmall"
                    android:layout_marginTop="@dimen/sidhe_spacing_2"/>

                <TextView
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:text="This is an example of the SIDHE design system implementation."
                    android:textAppearance="@style/Sidhe.TextAppearance.Body"
                    android:layout_marginTop="@dimen/sidhe_spacing_4"/>
            </LinearLayout>
        </com.google.android.material.card.MaterialCardView>

        <!-- Alert Examples -->
        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="Alerts"
            android:textAppearance="@style/Sidhe.TextAppearance.Heading3"
            android:layout_marginTop="@dimen/sidhe_spacing_8"/>

        <!-- Info Alert -->
        <LinearLayout
            style="@style/Sidhe.Alert.Info"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="@dimen/sidhe_spacing_4"
            android:orientation="horizontal">

            <View
                android:layout_width="@dimen/sidhe_stroke_width_medium"
                android:layout_height="match_parent"
                android:background="@color/sidhe_color_secondary_500"
                android:layout_marginEnd="@dimen/sidhe_spacing_4"/>

            <TextView
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="This is an informational message."
                android:textAppearance="@style/Sidhe.TextAppearance.Body"/>
        </LinearLayout>

        <!-- Success Alert -->
        <LinearLayout
            style="@style/Sidhe.Alert.Success"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="@dimen/sidhe_spacing_4"
            android:orientation="horizontal">

            <View
                android:layout_width="@dimen/sidhe_stroke_width_medium"
                android:layout_height="match_parent"
                android:background="@color/sidhe_color_green_200"
                android:layout_marginEnd="@dimen/sidhe_spacing_4"/>

            <TextView
                android:layout_width="0dp"
                android:layout_height="wrap_content"
                android:layout_weight="1"
                android:text="Operation completed successfully."
                android:textAppearance="@style/Sidhe.TextAppearance.Body"/>
        </LinearLayout>

        <!-- Form Example -->
        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="Form Elements"
            android:textAppearance="@style/Sidhe.TextAppearance.Heading3"
            android:layout_marginTop="@dimen/sidhe_spacing_8"/>

        <com.google.android.material.textfield.TextInputLayout
            style="@style/Sidhe.TextInputLayout"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="@dimen/sidhe_spacing_4"
            android:hint="Full Name">

            <com.google.android.material.textfield.TextInputEditText
                style="@style/Sidhe.TextInputEditText"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:inputType="textPersonName"/>
        </com.google.android.material.textfield.TextInputLayout>

        <!-- Button Examples -->
        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="Buttons"
            android:textAppearance="@style/Sidhe.TextAppearance.Heading3"
            android:layout_marginTop="@dimen/sidhe_spacing_8"/>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:orientation="vertical"
            android:layout_marginTop="@dimen/sidhe_spacing_4">

            <com.google.android.material.button.MaterialButton
                style="@style/Sidhe.Button.Primary"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="Primary Button"/>

            <com.google.android.material.button.MaterialButton
                style="@style/Sidhe.Button.Secondary"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginTop="@dimen/sidhe_spacing_4"
                android:text="Secondary Button"/>

            <com.google.android.material.button.MaterialButton
                style="@style/Sidhe.Button.Ghost"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_marginTop="@dimen/sidhe_spacing_4"
                android:text="Ghost Button"/>
        </LinearLayout>
    </LinearLayout>
</androidx.core.widget.NestedScrollView>


            
