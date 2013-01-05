# Heroku Favicon

![favicon-16x16](https://github.com/heroku/favicon/raw/master/favicon.iconset/icon_16x16.png) ![favicon-32x32](https://github.com/heroku/favicon/raw/master/favicon.iconset/icon_32x32.png)

The assets for Heroku's favicon live here. To generate updated assets from
`source` make sure you have Adobe Photoshop and [Icon
Slate][icon-slate] installed.

1. Export the 16x16 and 32x32 icon via Save for Web in Photoshop (disable
   [Convert to sRGB][convert-to-srgb]) to the `favicon.iconset`
   directory.
2. Open the `favicon.iconsproj` file with Icon Slate and drag the new assets
   from `favicon.iconset` to the correct canvas. 
3. Build the icon (the only format required is `.ico`).

To include the favicon in your application you can:

* Use the Rails helper: [`favicon_link_tag`][favicon-helper]
* Include the favicon tag manually:
  ```
  <link href="/favicon.ico" rel="shortcut icon" type="image/vnd.microsoft.icon" />
  ```

[icon-slate]: http://itunes.apple.com/app/icon-slate/id439697913?mt=12&ls=1
[convert-to-srgb]: http://cl.ly/image/3K0h3R1H343P
[favicon-helper]: http://api.rubyonrails.org/classes/ActionView/Helpers/AssetTagHelper.html#method-i-favicon_link_tag
