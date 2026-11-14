# Scout distribution

Public update metadata for Scout, the local Windows launcher and search app.
Scout's source repository remains private.

The stable and preview channels are signed with the publisher's RSA-PSS key.
The app verifies its pinned publisher key before trusting a channel descriptor.

No installer release is published yet. A valid empty channel means that no
update is currently offered; it does not download or install anything.

Future installer assets and release notes will be published here after package
validation. Updates notify the user and require confirmation. Personal indexes,
models, credentials, source code and local profiles are not part of this repository.

Channel paths: `channels/stable.json` and `channels/preview.json`.
`publisher-key.spki` is the public verification key. The private signing key
is retained in the publisher's non-exportable Windows key store.
