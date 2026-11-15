# Radio signature interchange

A proposal for a shared file of radio signatures. An app can recognize the radios another app has already learned, and an app can publish a library other apps can read.

This is a proposal for comment. It is not an adopted standard.

The current document is RSI-1, Release 4, 15 November 2026: [Radio signature interchange](docs/papers/Radio_Signature_Interchange.pdf). A shared library uses the suffix `.rsi`. The name before that suffix is up to the publisher.

Fieldwatch is the first implementation. Releases through 1.1.44 already read a library close to this file. Fieldwatch 1.2.0 is the release that will conform. Fieldwatch™ is a trademark of Off Grid Pete LLC. Registration pending.

## Taking part

Comment here, or open an issue. A profile for a radio you already receive needs the observation fields, the rule kinds, and the test vectors. An empty profile is not a contribution.

A project can also take part by implementing the matcher, or by writing and publishing a library other apps can read.

There is no fee and no separate organization.

## Badge

An app that reads or writes a `radio-signatures` file for RSI-1 may show this badge. The badge is that app's claim. This repository does not check it.

![RSI-1 signatures supported](badges/RSI.svg)

```markdown
[![RSI-1 signatures supported](https://raw.githubusercontent.com/OffGridPete/radio-signature-interchange/main/badges/RSI.svg)](https://github.com/OffGridPete/radio-signature-interchange)
```

## Building the PDF

From the repository root, with Python 3 and reportlab:

```
python3 docs/papers/build_signature_spec.py
```
