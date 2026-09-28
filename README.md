openai says my FIDO2 hardware key is a passkey. also i need two.
I built a physical ESP32-S3 FIDO2/CTAP 2.1 security key for OpenAI Daybreak. It registers and authenticates correctly, but OpenAI classifies it as a passkey rather than a hardware security key.
OpenAI Support says MDS listing and attestation are not documented requirements, there is no documented arbitrary-AAGUID allowlist, and the workaround for a working physical key that is not recognized is to use a different key.
Support also clarified the practical enrollment requirement: Advanced Account Security needs two sign-in methods, while Daybreak disallows software/synced passkeys. So individual Daybreak effectively requires two qualifying physical hardware keys.
The full post is in index.html.
GitHub Pages
Publish from:
    • Branch: main
    • Folder: / (root)
Expected URL:
https://voidnullvalue.github.io/openai-fido2/
