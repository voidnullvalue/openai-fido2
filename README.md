# openai says my FIDO2 hardware key is a passkey

I built a physical ESP32-C3 FIDO2/CTAP 2.1 security key. OpenAI registers it and authenticates with it, then classifies it as a passkey, which means Daybreak does not count it as a hardware key.

The actual post lives in `index.html` and is plain HTML/CSS with no build step.

## GitHub Pages

Publish from:

- Branch: `main`
- Folder: `/ (root)`

Expected URL:

https://voidnullvalue.github.io/openai-fido2/

## What this covers

```text
ESP32-C3 / Pico FIDO2 6.6
USB HID
CTAP 2.1 / FIDO2 / U2F
self-assigned AAGUID
self-attestation
OpenAI registration works
OpenAI authentication works
OpenAI classification: Passkey
Daybreak hardware-key requirement: not satisfied
```

The post also documents the unrelated Void Linux udev failure that initially made the key invisible to Chromium, and why I think relying on vendor attestation as a hidden definition of "hardware" is a bad policy boundary.
