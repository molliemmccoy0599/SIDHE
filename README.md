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
/**
 * SIDHE Design System - Style Dictionary Configuration
 *
 * This configuration file defines how to transform the source tokens
 * into platform-specific formats.
 */

const StyleDictionary = require('style-dictionary');

// Custom transforms
StyleDictionary.registerTransform({
  name: 'size/px',
  type: 'value',
  matcher: (token) => {
    return token.value.toString().endsWith('px');
  },
  transformer: (token) => {
    return token.value.toString().replace('px', '');
  }
});

// Custom formats
StyleDictionary.registerFormat({
  name: 'json/nested',
  formatter: function(dictionary) {
    return JSON.stringify(dictionary.tokens, null, 2);
  }
});

// Style Dictionary Configuration
module.exports = {
  source: ['tokens/**/*.json'],
  platforms: {
    // Web: CSS Variables
    css: {
      transformGroup: 'css',
      buildPath: 'dist/web/',
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
      buildPath: 'dist/web/',
      files: [{
        destination: 'sidhe-tokens.scss',
        format: 'scss/variables',
        options: {
          outputReferences: true
        }
      }]
    },
    
    // Android: XML Resources
    android: {
      transformGroup: 'android',
      buildPath: 'dist/android/src/main/res/values/',
      files: [
        {
          destination: 'sidhe_colors.xml',
          format: 'android/colors',
          filter: {
            type: 'color'
          }
        },
        {
          destination: 'sidhe_dimens.xml',
          format: 'android/dimens',
          filter: {
            type: 'size'
          }
        }
      ]
    },
    
    // iOS: Swift Constants
    ios: {
      transformGroup: 'ios',
      buildPath: 'dist/ios/',
      files: [
        {
          destination: 'SidheColors.swift',
          format: 'ios/colors.swift',
          className: 'SidheColors',
          filter: {
            type: 'color'
          }
        },
        {
          destination: 'SidheTypography.swift',
          format: 'ios/swift/any',
          className: 'SidheTypography',
          filter: {
            type: 'typography'
          }
        },
        {
          destination: 'SidheSpacing.swift',
          format: 'ios/swift/any',
          className: 'SidheSpacing',
          filter: {
            type: 'size'
          }
        }
      ]
    },
    
    // JSON for reference
    json: {
      transformGroup: 'js',
      buildPath: 'dist/json/',
      files: [
        {
          destination: 'sidhe-tokens.json',
          format: 'json/nested'
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
      - 'tokens/**/*.json'
      - 'config.js'
  pull_request:
    branches: [ main ]
  workflow_dispatch:

jobs:
  build:
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

      - name: Build all tokens
        run: npm run build:all

      - name: Upload build artifacts
        uses: actions/upload-artifact@v3
        with:
          name: token-dist
          path: dist/
          retention-days: 7

  deploy:
    needs: build
    if: github.ref == 'refs/heads/main'
    runs-on: ubuntu-latest
    steps:
    
## Installation and Usage 
npm install @sidhe/design-system
<link rel="stylesheet" href="path/to/sidhe-tokens.css">

res/values/sidhe_colors.xml
res/values/sidhe_dimens.xml
res/values/sidhe_typography.xml

SIDHEColors.swift
SIDHETypography.swift
SIDHESpacing.swift

/* CSS */
.button {
  background-color: var(--sidhe-color-primary-500);
  font-size: var(--sidhe-font-size-md);
  padding: var(--sidhe-spacing-3);
  border-radius: var(--sidhe-radius-base8);
}


<!-- XML -->
<Button
  android:textColor="@color/sidhe_color_primary_500"
  android:padding="@dimen/sidhe_spacing_3" />
  
// Swift
label.textColor = SIDHEColors.primary.color500
button.contentEdgeInsets = UIEdgeInsets(
  top: SIDHESpacing.spacing3,
  left: SIDHESpacing.spacing3,
  bottom: SIDHESpacing.spacing3, 
  right: SIDHESpacing.spacing3
)

## Implementation Examples

## Web (CSS variable)
/* Button Component Example */
.button {
  /* Colors */
  background-color: var(--sidhe-color-primary-500);
  color: white;
  
  /* Typography */
  font-family: var(--sidhe-font-family-primary);
  font-size: var(--sidhe-font-size-md);
  font-weight: var(--sidhe-font-weight-medium);
  
  /* Layout */
  padding: var(--sidhe-spacing-3) var(--sidhe-spacing-6);
  border-radius: var(--sidhe-radius-base8);
  
  /* Effects */
  box-shadow: var(--sidhe-effect-elevation-e1);
}

.button:hover {
  background-color: var(--sidhe-color-primary-400);
  box-shadow: var(--sidhe-effect-elevation-e2);
}

/* Card Component Example */
.card {
  background-color: white;
  border-radius: var(--sidhe-radius-base8);
  padding: var(--sidhe-spacing-6);
  box-shadow: var(--sidhe-effect-elevation-e2);
}

.card-title {
  font-family: var(--sidhe-font-family-secondary);
  font-size: var(--sidhe-font-size-2xl);
  font-weight: var(--sidhe-font-weight-bold);
  margin-bottom: var(--sidhe-spacing-2);
}

/* Alert Component Example */
.alert {
  padding: var(--sidhe-spacing-4);
  border-radius: var(--sidhe-radius-base4);
  margin-bottom: var(--sidhe-spacing-4);
}

.alert-info {
## IOS (Swift) 
import UIKit

// Button Component Extension
extension UIButton {
    func applySIDHEPrimaryStyle() {
        backgroundColor = SIDHEColors.primary.color500
        setTitleColor(.white, for: .normal)
        titleLabel?.font = UIFont(name: SIDHETypography.fontFamily.primary, size: SIDHETypography.fontSize.md)
        layer.cornerRadius = SIDHERadius.base8
        contentEdgeInsets = UIEdgeInsets(
            top: SIDHESpacing.spacing3,
            left: SIDHESpacing.spacing6,
            bottom: SIDHESpacing.spacing3,
            right: SIDHESpacing.spacing6
        )
        
        // Add shadow
        layer.shadowColor = UIColor.black.cgColor
        layer.shadowOffset = CGSize(width: 0, height: 1)
        layer.shadowRadius = 3
        layer.shadowOpacity = 0.1
    }
    
    func applySIDHESecondaryStyle() {
        backgroundColor = SIDHEColors.secondary.color500
        setTitleColor(.white, for: .normal)
        titleLabel?.font = UIFont(name: SIDHETypography.fontFamily.primary, size: SIDHETypography.fontSize.md)
        layer.cornerRadius = SIDHERadius.base8
        contentEdgeInsets = UIEdgeInsets(
            top: SIDHESpacing.spacing3,
            left: SIDHESpacing.spacing6,
            bottom: SIDHESpacing.spacing3,
            right: SIDHESpacing.spacing6
        )
    }
}

// Text Style Extensions
extension UILabel {
    func applySIDHEHeading1Style() {
        font = UIFont(name: SIDHETypography.fontFamily.secondary, size: SIDHETypography.fontSize.xl4)
        textColor = SIDHEColors.neutral.color900
    }
    
    func applySIDHEHeading2Style() {
        font = UIFont(name: SIDHETypography.fontFamily.secondary, size: SIDHETypography.fontSize.xl3)
        textColor = SIDHEColors.neutral.color900
    }
    
    func applySIDHEBodyStyle() {
        font = UIFont(name: SIDHETypography.fontFamily.primary, size: SIDHETypography.fontSize.md)
        textColor = SIDHEColors.neutral.color800
    }
}

// Card View Extension
extension UIView {
    func applySIDHECardStyle() {
        backgroundColor = .white
        layer.cornerRadius = SIDHERadius.base8
        
        // Add shadow
        layer.shadowColor = UIColor.black.cgColor
        layer.shadowOffset = CGSize(width: 0, height: 2)
        layer.shadowRadius = 6
        layer.shadowOpacity = 0.1
    }
}

// Example Usage
class ExampleViewController: UIViewController {
    override func viewDidLoad() {
        super.viewDidLoad()
        
        // Create a card
        let cardView = UIView(frame: CGRect(x: 20, y: 100, width: view.bounds.width - 40, height: 200))
        cardView.applySIDHECardStyle()
        view.addSubview(cardView)
        
        // Add a title to the card
        let titleLabel = UILabel(frame: CGRect(x: 16, y: 16, width: cardView.bounds.width - 32, height: 30))
        titleLabel.applySIDHEHeading2Style()
        titleLabel.text = "SIDHE Design System"
        cardView.addSubview(titleLabel)
        
        // Add a description
        let descriptionLabel = UILabel(frame: CGRect(x: 16, y: 54, width: cardView.bounds.width - 32, height: 60))
        descriptionLabel.a

        import SwiftUI

// Text Styles
struct SIDHETextStyles {
    struct Heading1: ViewModifier {
        func body(content: Content) -> some View {
            content
                .font(.custom(SIDHETypography.fontFamily.secondary, size: SIDHETypography.fontSize.xl4))
                .foregroundColor(Color(SIDHEColors.neutral.color900))
                .lineSpacing(8)
        }
    }
    
    struct Heading2: ViewModifier {
        func body(content: Content) -> some View {
            content
                .font(.custom(SIDHETypography.fontFamily.secondary, size: SIDHETypography.fontSize.xl3))
                .foregroundColor(Color(SIDHEColors.neutral.color900))
                .lineSpacing(6)
        }
    }
    
    struct BodyText: ViewModifier {
        func body(content: Content) -> some View {
            content
                .font(.custom(SIDHETypography.fontFamily.primary, size: SIDHETypography.fontSize.md))
                .foregroundColor(Color(SIDHEColors.neutral.color800))
                .lineSpacing(4)
        }
    }
}

// Button Styles
struct SIDHEPrimaryButtonStyle: ButtonStyle {
    func makeBody(configuration: Configuration) -> some View {
        configuration.label
            .padding(.vertical, SIDHESpacing.spacing3)
            .padding(.horizontal, SIDHESpacing.spacing6)
            .background(
                configuration.isPressed ? 
                    Color(SIDHEColors.primary.color400) : 
                    Color(SIDHEColors.primary.color500)
            )
            .foregroundColor(.white)
            .cornerRadius(SIDHERadius.base8)
            .shadow(color: Color.black.opacity(0.1), radius: 3, x: 0, y: 1)
    }
}

// View Extensions
extension View {
    func sidheHeading1() -> some View {
        modifier(SIDHETextStyles.Heading1())
    }
    
    func sidheHeading2() -> some View {
        modifier(SIDHETextStyles.Heading2())
    }
    
    func sidheBodyText() -> some View {
        modifier(SIDHETextStyles.BodyText())
    }
}

// Card Component
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
            .shadow(color: Color.black.opacity(0.1), radius: 6, x: 0, y: 2)
    }
}

// Example Usage
struct ContentView: View {
    var body: some View {
        VStack(alignment: .leading, spacing: SIDHESpacing.spacing6) {
            Text("SIDHE Design System")
                .sidheHeading1()
            
            SIDHECard {
                VStack(alignment: .leading, spacing: SIDHESpacing.spacing4) {
                    Text("SwiftUI Components")
                        .sidheHeading2()
                    
                    Text("These components are built using the SIDHE design tokens to ensure consistent styling across the app.")
                        .sidheBodyText()
                    
                    Button("Learn More") {
                        // Action
                    }
                    .buttonStyle(SIDHEPrimaryButtonStyle())
                    .padding(.top, SIDHESpacing.spacing2)
                }
            }
        }
        .padding(SIDHESpacing.spacing6)
    }
}

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


## Part 2: Reflection – Tokenizing a Brand's Style Guide
1. Benefits Realized
It was/is convient to have all of the colors and other styles in one refined place. However I did miss somewhat of the ability to add new things etc in an easier way than putting them in the library/guide yes of course you are still able to edit things outside of guide but it is just more constrained overall.



2. Drawbacks and Challenges
This was the worst project for me with constant frustration met across the board, the video of how to do the demo was never shared and I found myself floundering as I cannot learn something by just watching or attempting to quickly follow along. As for Drawbacks of even having a token system like this, is that it over complicates absolutely everything leading to little to no flexibility in changes or shifts that need to be made and creates confines that are smothering. The amount of stress and also just sleep that was lost on this project is ridiculous, I found it to be very difficult for very little to absolutely no pay off.

I found myself looking at my work then at my peers then to the internet to find some sort of answer only to come back to the same place that it just wouldn't work whether that be a bit of code falling off the end or what to have it read correctly felt/feels nearly impossible. After running out of questions on Claude as well as sources on the internet I turned to me peers for support to help me solve the issue.

4. Version Control and Governance
With control and anybody even making a slight change the code can stop working and it somthing I would be concerned about when functioning as a unite on something such as this, there is just so much cahnce of an error and I worry about something going wrong. In terms of working by myself its easy to go back in delete something then reaprroach it with new code or information, with others its not always the case. For instance as I work alone I rarely do push or pulls as I am the sole person in charge however in a team setting these are necessary to keep code organized and avoid unnecessary errors. 

5. Automation and Pipeline Considerations
Keepig consistent style guides is key and I almost feel as though why my automation and other portions didn't work is because of change breaking and small little lines that break other portions of code along the way. Though I do definitly think there is comofort if say code was the primary thing that you did as it would be easier to catch errors etc. 

6. Tokens in the Wild
From what I have seen many companies from apple to google tokenize as it creates easy accesible short cuts to components that both coders can use such as what can be seen here in the github and designers can mess around with such as a particular logo, type face, or radius it quickly makes things uniform. We were recently going over Apple's Material guide which in my opinion is an exccellent example of both a style guide and a token system with the website/library covering an extensive array of materials. 
