# Web

_You can find the scaffolding for this example in `crates/web`.
The finished example code is available in the `finished` branch._

In this tutorial you'll get familiar with:

* Interacting with a WASM application from JavaScript
* `wasm-bindgen` tooling to handle more complex types passed over the boundary
* web workers to run WebAssembly separate from the main web page.

Next we build a web application that processes images client-side in the browser.
No server processing involved.

We re-use the same Rust crate to apply the image filter,
but this time load the image directly from a binary blob.
That binary blob is passed in from the JavaScript side.