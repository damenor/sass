### Mixins, functions and variables for SASS

* Install

```
  npm install --save-dev @damenor/sass
    
  or

  npm i -D @damenor/sass
```

* Import in file .scss

```scss

  /***** SET VARIABLES HERE *****/

  @import '<YOUR_PROJECT_PATH>/node_modules/@damenor/sass/index.scss'; // For SASS utils

  @import '<YOUR_PROJECT_PATH>/node_modules/@damenor/sass/dist/styles.min.css'; // For CSS class

```

## DOCS 

### Default Variables

#### Global
```scss
  $reset: true;
  $animated: true;
  $grid-columns: 12 !default;

  $fonts: () !default; // Values: (Kufan, Roboto, Ranchers)

  $navbar-height: 3rem;

  $footer-height: 2rem;

  $container-height: calc(100vh - #{$navbar-height} - #{$footer-height});
```

#### Colors
```scss
  $color-theme-primary: #CF649A;
  $color-theme-primary-light: lighten(#CF649A, 5);
  $color-theme-secondary: #37474f;
  $color-theme-light: #ecf0f1;
  $color-theme-danger: #e74c3c;
  $color-theme-info: #2980b9;
  $color-theme-success: #2ecc71;
  $color-theme-warning: #f39c12;
```

#### Generate class
```scss
  $generate-class: false;
  $generate-class-grid: false;
  $generate-class-flexbox: false;
  $generate-class-padding: false;
  $generate-class-margin: false;
  $generate-class-geometry: false;
  $generate-class-bg-color: false;
  $generate-class-text-color: false;
```

#### Breakpoints
```scss
  $breakpoint-xxs: 320;
  $breakpoint-xs: 544;
  $breakpoint-sm: 768;
  $breakpoint-md: 992;
  $breakpoint-lg: 1200;
  $media-query-breakpoints: (
    xxs: $breakpoint-xxs,
    xs: $breakpoint-xs,
    sm: $breakpoint-sm,
    md: $breakpoint-md,
    lg: $breakpoint-lg
  );
```
