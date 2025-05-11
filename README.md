# QRCode.js

QRCode.js is a JavaScript library for generating QR codes. QRCode.js supports cross-browser compatibility with HTML5 Canvas and table tag in the DOM.

QRCode.js has no dependencies.

This fork has the following patches applied:

- https://github.com/davidshimjs/qrcodejs/pull/279
- https://github.com/davidshimjs/qrcodejs/pull/295
- https://github.com/davidshimjs/qrcodejs/pull/305
- https://github.com/davidshimjs/qrcodejs/pull/307
- https://github.com/davidshimjs/qrcodejs/pull/310

## Basic Usages
```
<div id="qrcode"></div>
<script type="text/javascript">
new QRCode(document.getElementById("qrcode"), "https://example.com");
</script>
```

or with some options

```
<div id="qrcode"></div>
<script type="text/javascript">
var qrcode = new QRCode(document.getElementById("qrcode"), {
	text: "https://example.com",
	width: 128,
	height: 128,
	colorDark: "#000000",
	colorLight: "#ffffff",
	correctLevel: QRCode.CorrectLevel.H,
    useUtf8Bom: false,
    borderWidth:2,
    autoAlignment:false,
});
</script>
```

and you can use some methods

```
qrcode.clear(); // clear the code.
qrcode.makeCode("https://example.com"); // make another code.
```

## Browser Compatibility

IE6~10, Chrome, Firefox, Safari, Opera, Mobile Safari, Android, Windows Mobile, etc.

## License

MIT License
