# sass-webfont

This is a reusable webfont scss package.

## Usage

    @import "node_modules/sass-webfont/_manifest.scss";

    // Define font
    @include WebFontDefine("default", "NovaSlim", "fonts/NovaSlim.tff");

    // Use font
    html {
      body {
        font-family: WebFont("default");
      }
    }

If you attempt to use a webfont that is not defined, you'll see an error like:

    WARNING: Invalid attempt to use unknown font alias 'dfault'
             on line 46 of node_modules/sass-webfont/src/webfont.scss

Notice that the alias used when using a font shouldn't be the name of the
font. If you want a simple font-name based call, use a different package.

Font aliases should be meaningful high level names ('default', 'header', etc)
which are easily remapped to different fonts by updating the `WebFontDefine`
call.

## Install

    npm init
    npm install shadowmint/sass-webfont --save

Now add an import statement to your scss file, like this:

    @import "../node_modules/sass-webfont/_manifest.scss";

## Development

To run tests:

    scss  _test.scss

Also see the `demo` folder.
