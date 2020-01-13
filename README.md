# browser-logging-client

Listens for logs from [browser-logging-server](https://www.npmjs.com/package/browser-logging-server).

This is useful for retrieving Cypress UI test browser logs.

Any message sent to `console.log`, `console.warn` and `console.error` will be sent to and logged by the logging server.

### Usage

Add the dependency to your project with:

```
yarn add browser-logging-client
```

or

```
npm install browser-logging-client
```

Then import & initialise at the root of your application.

```js
import browserLoggingClient from "browser-logging-client";
browserLoggingClient.initialise();
```

Note calling `initialise` more than once has no effect.

Ensure the [server](https://www.npmjs.com/package/browser-logging-server) is running before starting your application.

## Publishing

Install `np` - https://github.com/sindresorhus/np:

```
yarn global add np
```

Run `np` and follow instructions.

## License

[MIT](https://opensource.org/licenses/MIT) License.
