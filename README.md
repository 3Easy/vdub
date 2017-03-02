## VDub. Viewport Scalable Type.

Inspired by Craig Sharkie’s [vw + vh === vnice](http://webdirections.org/respond16/speakers/craig-sharkie.html) talk at Respond16, in turn inspired by Mike Riethmuller’s blog post circa 2015 entitled [Precise Control Responsive Typography](http://madebymike.com.au/writing/precise-control-responsive-typography/), here’s my shot at a viewport scalable type mixin `@mixin vdub`.

## Requirements

- [Sass](https://github.com/sass/sass) 3.4+ or [LibSass](https://github.com/sass/libsass) 3.1+

## Installation

Install VDub with [Bower](http://bower.io).

- Install into the current directory…

  ```bash
  vdub install
  ```
  
- Import at the beginning of your stylesheet…

  ```scss
  @import "vdub/vdub";
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
