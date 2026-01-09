# AWS VPN Tab Close Chrome Extension
An extension to detect and close the authentication tab left open by AWS VPN. This fork allows Chrome to return focus to the tab that was previously active in the window, instead of always focusing on the rightmost tab after closing the AWS VPN tab.

### Install

This is a fork of the extension in the [Chrome Web Store](https://chromewebstore.google.com/detail/eeohkjpjmohadfbgaghdofdphnjhidfg?hl=en-GB). To install this version:

1. Go the the extensions page (`chrome://extensions`) and [enable `Developer mode`](https://developer.chrome.com/docs/extensions/get-started/tutorial/hello-world#load-unpacked).
2. Either:
    - Download the zip and just drag it onto the extensions page (you may need to refresh the page after enable developer mode if it tries to download the zip); or
    - Clone this repo and click `Load unpacked` and point it to the repo directory

### Permissions
This extension requires only `host permission` so that it can detect a tab navigating to `http://127.0.0.1:35001/` this is the AWS VPN Client showing you a success message.

Chrome doesn't "activate" this extension for any other URL or any other port running on 127.0.0.1

See the [AWS Client VPN User Guide](https://docs.aws.amazon.com/vpn/latest/clientvpn-user/client-vpn-user-what-is.html) for more information.

### Privacy

This extension does **not** collect **any** information.

### Build

Use `build.sh` to build a standardised zip file that can be uploaded to the Chrome Web Store.
