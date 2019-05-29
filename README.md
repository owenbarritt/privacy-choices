# Privacy Choices

Privacy Choices is a JavaScript library that allows you to give the users of your website choices regarding the use of cookies and other web storage technologies on their device. Configured correctly, this library should be GDPR-compliant.

## Live demo

<http://code.benthomas.me/privacy-choices>

## Development

[![CircleCI](https://circleci.com/gh/benjeh32/privacy-choices.svg?style=svg)](https://circleci.com/gh/benjeh32/privacy-choices)

### Prerequisites

- [Node.js](https://nodejs.org/)

### Dependencies

Install development dependencies:

```console
npm install
```

### Building

To build once in production mode:

```console
npm run build

```

To start the live-updating development build that will rebuild whenever a change is made to the JavaScript or CSS:

```console
npm run start
```

Either way, the library bundle that is built will be at `build/privacy-choices.bundle.js`.

### Using

After it is built, reference `build/privacy-choices.bundle.js` and use the library like normal. The example page at `examples/index.html` does this.

***Note:** This library stores the user's preferences in a cookie. Many popular browsers no longer support the use of cookies for `file://...` or `http://localhost/...` browsing so this may make development trickier. Most of the original development on this library was done using Microsoft Edge, which doesn't seem to mind local cookies.*