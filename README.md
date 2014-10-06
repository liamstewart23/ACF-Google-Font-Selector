# ACF Google Font Selector Field

Welcome to the the Google Font Selector Field for Advanced Custom Fields.

This plugin allows you to create a Google font selector field with different options. The plugin also creates the font request in the theme header. Font variants and charsets can be selected separately to make font loading more flexible and optimized.

Font options added to any options page will always be enqueues. Any fonts added to post pages will only be enqueued when that specific post is displayed.

This ACF field type is compatible with **ACF 4** and **ACF 5**.

## Usage

Once installed the list of Google Fonts will be retrieved from a static file included in the plugin. If you would like the list to be pulled from the Google API you will need to define your API key. You can do this in the theme's function file for example.

`define( 'ACFGFS_API_KEY', 'your_google_api_key' );`

 It's super easy to get an API key, just head on over to the [Google API Console](http://cloud.google.com/console), create a new project and get a browser api key.


The `ACFGFS_REFRESH` constant can also be defined, it controls how frequently the plugin checks the Google API for updates. The value is in seconds, 86400 would be a day. The default is set to 3 days.

`define( 'ACFGFS_REFRESH', 259200 );`

If you would like to disable the automatic enqueueing of fonts you can use the `ACFGFS_NOENQUEUE` constant. The fonts are only enqueued automatically when this constant is not defined. Define the constant to disable enqueueing.

`define( 'ACFGFS_NOENQUEUE', true );`


-----------------------

* WordPress Repository: https://wordpress.org/plugins/acf-google-font-selector-field/
* Support: https://wordpress.org/support/plugin/acf-google-font-selector-field
