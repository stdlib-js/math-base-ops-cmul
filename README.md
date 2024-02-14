<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# cmul

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Multiply two double-precision complex floating-point numbers.

<section class="intro">

</section>

<!-- /.intro -->



<section class="usage">

## Usage

```javascript
import cmul from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-ops-cmul@v0.2.0-esm/index.mjs';
```

#### cmul( z1, z2 )

Multiplies two double-precision complex floating-point numbers.

```javascript
import Complex128 from 'https://cdn.jsdelivr.net/gh/stdlib-js/complex-float64@esm/index.mjs';
import real from 'https://cdn.jsdelivr.net/gh/stdlib-js/complex-real@esm/index.mjs';
import imag from 'https://cdn.jsdelivr.net/gh/stdlib-js/complex-imag@esm/index.mjs';

var z1 = new Complex128( 5.0, 3.0 );
var z2 = new Complex128( -2.0, 1.0 );

var v = cmul( z1, z2 );
// returns <Complex128>

var re = real( v );
// returns -13.0

var im = imag( v );
// returns -1.0
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="module">

import Complex128 from 'https://cdn.jsdelivr.net/gh/stdlib-js/complex-float64@esm/index.mjs';
var discreteUniform = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/random-base-discrete-uniform' ).factory;
import cmul from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-ops-cmul@v0.2.0-esm/index.mjs';

var rand;
var z1;
var z2;
var z3;
var i;

rand = discreteUniform( -50, 50 );
for ( i = 0; i < 100; i++ ) {
    z1 = new Complex128( rand(), rand() );
    z2 = new Complex128( rand(), rand() );
    z3 = cmul( z1, z2 );
    console.log( '(%s) * (%s) = %s', z1.toString(), z2.toString(), z3.toString() );
}

</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- C interface documentation. -->



<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/math-base/ops/cadd`][@stdlib/math/base/ops/cadd]</span><span class="delimiter">: </span><span class="description">add two double-precision complex floating-point numbers.</span>
-   <span class="package-name">[`@stdlib/math-base/ops/cdiv`][@stdlib/math/base/ops/cdiv]</span><span class="delimiter">: </span><span class="description">divide two complex numbers.</span>
-   <span class="package-name">[`@stdlib/math-base/ops/csub`][@stdlib/math/base/ops/csub]</span><span class="delimiter">: </span><span class="description">subtract two double-precision complex floating-point numbers.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-ops-cmul.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-ops-cmul

[test-image]: https://github.com/stdlib-js/math-base-ops-cmul/actions/workflows/test.yml/badge.svg?branch=v0.2.0
[test-url]: https://github.com/stdlib-js/math-base-ops-cmul/actions/workflows/test.yml?query=branch:v0.2.0

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-ops-cmul/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-ops-cmul?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-ops-cmul.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-ops-cmul/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-ops-cmul/tree/deno
[deno-readme]: https://github.com/stdlib-js/math-base-ops-cmul/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/math-base-ops-cmul/tree/umd
[umd-readme]: https://github.com/stdlib-js/math-base-ops-cmul/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/math-base-ops-cmul/tree/esm
[esm-readme]: https://github.com/stdlib-js/math-base-ops-cmul/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/math-base-ops-cmul/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-ops-cmul/main/LICENSE

<!-- <related-links> -->

[@stdlib/math/base/ops/cadd]: https://github.com/stdlib-js/math-base-ops-cadd/tree/esm

[@stdlib/math/base/ops/cdiv]: https://github.com/stdlib-js/math-base-ops-cdiv/tree/esm

[@stdlib/math/base/ops/csub]: https://github.com/stdlib-js/math-base-ops-csub/tree/esm

<!-- </related-links> -->

</section>

<!-- /.links -->
