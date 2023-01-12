---
title: Appearance settings
sidebar: cyclr_sidebar
permalink: console-appearance-settings
tags: [cyclr-config]

menus:
    cyclr-configuration:
        title: Appearance settings
        identifier: console-appearance-settings
        toggleonly: menutoggleonly
        weight: 3
---
{::options parse_block_html="true" /}
<section class="card">
These settings allow you to change the appearance of Cyclr when in Accounts, using LAUNCH or Marketplaces.

*Due to caching within Cyclr, allow 1 minute before the changes take effect.*


</section>
<section class="card">
## Application LESS Variables

The simplest way to alter the appearance of Cyclr is to change the values of LESS variables.

For example if the *body-background* is set to *#ccc* then the background of Cyclr will change to grey.

``` less
@body-background: #ccc;
```

![](/images/settings-appearance-less.png)


</section>
<section class="card">
## Application Custom CSS

If changing the LESS variables is insufficient to provide the customization that you require you can also include you own custom CSS block, this will be included alongside the Application LESS so you can use both as required.

For example to change the rounded buttons to squares you could use

``` css
.btn-rounded {
    border-radius: 0;
}
```

![](/images/settings-appearance-css.png)


</section>
<section class="card">
## Header HTML

Header HTML allows HTML & JavaScript to be injected into the header of the page.

``` html
<h1>This is a header</h1>
```

![](/images/settings-appearance-header-html.png)


</section>
<section class="card">
## Footer HTML

Footer HTML allows HTML & JavaScript to be injected into the footer of the page.

``` html
<h1>This is a footer</h1>
```

![](/images/settings-appearance-footer-html.png)


</section>
<section class="card">
## Launch Complete HTML

Launch Complete HTML allows for the changing of HTML & JavaScript that is displayed at the end of the install process for LAUNCH and Marketplace. For more information, see [Handling Launch Callback](/handling-callback).


</section>
<section class="card">
## Connector Callback Error HTML

Connector Callback Error HTML allows for the changing of the HTML that is displayed when an error occurs when trying to authenticate a connector.

The error and error description, returned by the 3rd party, can be used within the HTML by including the {% raw %}{{error}} and {{error_description}}{% endraw %} merge fields. For example:

``` html
<p>The following error has occurred: {% raw %}{{error}} - {{error_description}}{% endraw %}</p>
```

</section>