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
  "description": "SIDHE Design System Tokens",
  "main": "index.js",
  "scripts": {
    "build": "style-dictionary build --config config.js",
    "clean": "rm -rf dist",
    "build:web": "style-dictionary build --config config.js --platform css,scss",
    "build:android": "style-dictionary build --config config.js --platform android",
    "build:ios": "style-dictionary build --config config.js --platform ios",
    "build:all": "npm run clean && npm run build"
  },
  "keywords": [
    "design-system",
    "tokens",
    "sidhe"
  ],
  "author": "SIDHE Design Team",
  "license": "MIT",
  "dependencies": {
    "style-dictionary": "^3.8.0"
  }
}

## Github Actions Workflow 



## Installation and Usage 



## Implementation Examples

## Web (CSS variable)


## IOS (Swift) 



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
It was/is convient to have all of the colors and other styles in one refined place.



2. Drawbacks and Challenges
This was the worst project for me with constant frustration met across the board, the video of how to do the demo was never shared and I found myself floundering as I cannot learn something by just watching or attempting to quickly follow along. As for Drawbacks of even having a token system like this, is that it over complicates absolutely everything leading to little to no flexibility in changes or shifts that need to be made and creates confines that are smothering. The amount of stress and also just sleep that was lost on this project is ridiculous, I found it to be very difficult for very little to absolutely no pay off. 

3. Version Control and Governance
With control and anybody even making a slight change the code can stop working and it somthing I would be concerned about when functioning as a unite on something such as this, there is jsut so much room for error and 

4. Automation and Pipeline Considerations

5. Tokens in the Wild

