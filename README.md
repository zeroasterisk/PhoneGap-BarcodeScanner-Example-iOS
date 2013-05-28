Example iOS PhoneGap Application with a working BarcodeScanner Plugin

Instructions
================

Take a look at this commit:
https://github.com/zeroasterisk/PhoneGap-BarcodeScanner-Example-iOS/commit/69f3300fe77ba5af6ad576d517b3b78406a00a80

Specifically:

Installed the plugin (in a handful of paths) but kept the one which worked.
Implemented a basic JS scanner code to demonstrate functionality:
auto-runs on load,
auto-reloads on error,
alerts on success/failure/cancel.

NOTE: the comments on the barcodescanner.js and index.js,
both mention my customization of the define/require object paths.
I could not get the demo/example paths to work, after several permutations.

Copied Files:

* barcodescanner/Plugins/com.phonegap.plugins.barcodescanner/...[all files]...
* barcodescanner/Resources/scannerOverlay.xib

Edited Files:

* barcodescanner/config.xml (added single plugin line)
* www/js/barcodescanner.js (manually changed the path for the define)
* www/index.html (included barcodescanner.js beforehand)
* www/js/index.js (auto-testable app.scan() method)
