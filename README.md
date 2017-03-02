## VDub. Viewport Scalable Type.

Inspired by Craig Sharkie’s [vw + vh === vnice](http://webdirections.org/respond16/speakers/craig-sharkie.html) talk at Respond16, in turn inspired by Mike Riethmuller’s blog post circa 2015 entitled [Precise Control Responsive Typography](http://madebymike.com.au/writing/precise-control-responsive-typography/), here’s my shot at a viewport scalable type mixin `@mixin vdub`.

In a nut, this gives you fluid typography that scales on the size of the viewport. In detail, your base type sizes will scale between 12px and 24px, between a 400px and 1200px viewport. Optionally supply your own arguments to override those values.

## Requirements

- [Sass](https://github.com/sass/sass) 3.4+ or [LibSass](https://github.com/sass/libsass) 3.1+

## Installation

Install VDub with [Bower](http://bower.io).

- Install into the project…

  ```bash
  bower install vdub
  ```
  
- Import at the beginning of your stylesheet…

  ```scss
  @import "../bower_components/vdub/scss/_vdub.scss";
  ```
  
- Include the mixin…

	```scss
	@include vdub();
	```

- Optionally, include four arguments…

	```scss
	@include vdub(16, 32, 640, 1280);
	```

## The Mixin

The mixin optionally accepts four arguments `min_font`, `max_font`, `min_width`, and `max_width`. Sensible fallback values are built in, 12, 24, 400, and 1200. The order of arguments presumes you want to change font sizes first, and screen widths later.

## License

Copyright © 2017– [3Easy & Co.](http://3easy.org)
VDub is free software,
and may be redistributed under the terms specified in the [license](LICENSE.md).
