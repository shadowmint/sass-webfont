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

## Install

    npm init
    npm install shadowmint/sass-webfont --save

Now add an import statement to your scss file, like this:

    @import "../node_modules/sass-webfont/_manifest.scss";

## Development

To run tests:

    scss  _test.scss

Also see the `demo` folder.
