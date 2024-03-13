
# chrome-clientid-storage

This NPM package provides a simple and efficient way to generate or retrieve a persistent `clientId` using Chrome's local storage. It's designed to be used in Chrome extensions or web apps that require a unique identifier for their users or sessions.

## Features

- **Easy Integration**: Seamlessly integrates with Chrome extensions.
- **Persistent IDs**: Generates and retrieves persistent client IDs that are stored in Chrome's local storage.
- **Asynchronous API**: Utilizes modern JavaScript async/await syntax for better readability and efficiency.

## Installation

To install the package, run the following command in your project directory:

```bash
npm install chrome-clientid-storage
```

## Usage

Import the `getOrCreateClientId` function from the package and call it to retrieve or generate a new `clientId`. The function will return a `clientId` that is either retrieved from Chrome's local storage or newly generated if it does not exist.

```javascript
import { getOrCreateClientId } from 'chrome-clientid-storage';

async function demo() {
  const clientId = await getOrCreateClientId();
  console.log(`Client ID: ${clientId}`);
}

demo();
```

## Requirements

- This package is intended for use in Chrome extensions or web applications that have access to the `chrome.storage` API.
- Make sure your project is configured to support ES Module syntax (`import`/`export`).

## Contributing

Your contributions are welcome! If you'd like to contribute, please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
