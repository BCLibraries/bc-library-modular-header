# bc-library-modular-header
Stand-alone modular header for BC Library sites.

This header is built to be easily dropped into a Bootstrap v3 framework application, yet can be added to any web application or framework.

A [custom "slim" stylesheet](css/lib-header-custom-bootstrap3.css) is provided for applications that don't use Bootstrap v3. This stylesheet uses a specific id prefix added to every selector to it is safe to use for any application.

## Quick installation
The easiest recipe is to add the following link tags to the `<head>` section of your web application.

```
<link rel="stylesheet" href="/path/to/css/lib-header-custom-bootstrap3.css"/>
<link rel="stylesheet" href="/path/to/css/lib-header.css"/>
```

Then add the contents of [lib-header.html](lib-header.html) into the top of the `<body>` section of your application. The exact placement of the header html is dependant on the specific application but can generally be the very first section within the `<body>` section.

### Additional stylesheets

While not necessary for most cases, it is recommended to include both [OpenSans](https://fonts.google.com/specimen/Open+Sans) and [Font Awesome](http://fontawesome.io/) fonts to the application **if they aren't already included!**

Your application `<head>` should look like the following.

```
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Open+Sans:300,300i,400,400i,600,600i,700,700i,800,800i">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css">
<link rel="stylesheet" href="/path/to/css/lib-header-custom-bootstrap3.css"/>
<link rel="stylesheet" href="/path/to/css/lib-header.css"/>
```
|     :warning: Additional stylesheets can add additional load time to your application     |
| :---: |


## If Bootstrap v3 is already included with your application

Great! You can leave out the [custom "slim" stylesheet](css/lib-header-custom-bootstrap3.css) link from your `<head>` section since it provides the same styles as Bootstrap. Of course, nothing bad will happen if you leave this stylesheet included.

## Caution using Bootstrap v4!

This header doesn't yet work with Bootstrap v4 styles. 
