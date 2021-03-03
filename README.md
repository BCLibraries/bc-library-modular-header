# bc-library-modular-header
Stand-alone modular header for BC Library sites.

This header is built to be easily dropped into a Bootstrap v3 or v4 framework application, yet can be added to any web application or framework.

A [custom "slim" stylesheet](css/lib-header-custom-bootstrap3.css) is provided for applications that don't use Bootstrap. This stylesheet uses a specific id prefix added to every selector to it is safe to use for any application. This stylesheet can be ignored if your application currently uses Bootstrap v3 or v4. 

## Quick installation
The easiest recipe is to add the following link tags to the `<head>` section of your web application.

### If your application currently uses Bootstrap v3 or v4:
```
<link rel="stylesheet" href="https://library.bc.edu/theme/modular/header/css/lib-header.css"/>
```

### Otherwise, include the custom slim stylesheet:
```
<link rel="stylesheet" href="https://library.bc.edu/theme/modular/header/css/lib-header-custom-bootstrap3.css"/>
<link rel="stylesheet" href="https://library.bc.edu/theme/modular/header/css/lib-header.css"/>
```

Then copy/paste the contents of [lib-header.html](lib-header.html) into the top of the `<body>` section of your application. The exact placement of the header html is dependant on the specific application but can generally be the very first section within the `<body>` section.

### Additional stylesheets

While not necessary for most cases, it is recommended to include both [OpenSans](https://fonts.google.com/specimen/Open+Sans) and [Font Awesome](http://fontawesome.io/) fonts to the application **if they aren't already included!**

Your application `<head>` might look like the following:

```
<link rel="preconnect" href="https://fonts.gstatic.com">
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Open+Sans&display=swap">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css">
<link rel="stylesheet" href="https://library.bc.edu/theme/modular/header/css/lib-header-custom-bootstrap3.css"/>
<link rel="stylesheet" href="https://library.bc.edu/theme/modular/header/css/lib-header.css"/>
```
|     :warning: Additional stylesheets can add additional load time to your application     |
| :---: |

## Changing header features

There are a few easy and quick ways to change the behavior of the header.

### Force header content to 100% page/app width

This header is based on the [Bootstrap v3 grid system](https://getbootstrap.com/docs/3.3/css/#overview-container), which uses responsive fixed-width containers. Container width can also change depending on the viewing device, but follows well established media query values for common device breakpoints. 

To force the header to always fill 100% of the page/app width simply change the second line of the module html to use `container-fluid`.

From 

```
<div class="container">
```

To

```
<div class="container-fluid">
```

## If Bootstrap v3 or v4 is already included with your application

Great! You can leave out the [custom "slim" stylesheet](css/lib-header-custom-bootstrap3.css) link from your `<head>` section since it provides the same styles as Bootstrap. Of course, nothing bad will happen if you leave this stylesheet included.

## Using Bootstrap v5-beta

This module appears to work with early beta releases of Bootstrap v5, but future compatability isn't guaranteed.