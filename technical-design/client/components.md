# Component List

the directory structure of Component

> Login
> -- Login.tsx

## Components

`Component` is state-less render unit which is driven by props.

### ShellPage

`ShellPage` can show the background and the bottom description for icp license. also the `ShellPage` should be the root component for every page.

props:

+ background: color, image, null
+ icp: string, null, html string
+ children: default of react


## Widgets

`Widget` is self-contained `Component` and be used in `Page`.

### Login

props:

+ logoImageUrl
+ logoName

i81n keys:


### TwoFactor

## Pages

`Page` is the glue `Component` which bind the route and composite of `Component` and `Widget`.

### LoginPage