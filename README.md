# Push Express 🚀🔔

**Push Express** is a tool that simplifies the integration of Push Protocol product components into web projects. Although development began with the implementation of push notification services, it now supports a wide range of Push Protocol functionalities. It allows you to add components and services quickly using TypeScript or JavaScript, with support for Yarn and NPM.

## Features

- Adds components for all Push Protocol products with a single command.
- Supports both TypeScript and JavaScript.
- Automatically installs dependencies using Yarn, NPM, or manually.
- Simple integration with [Push Protocol](https://push.org/) to manage Web3 notifications, chats, and more.

## Installation (Optional)

To install **Push Express**, follow these steps:

### Install with npm

```bash
npm install -g push-express
```

### Install with Yarn

```bash
yarn global add push-express
```

## Usage

Once installed, you can use **Push Express** in your project to add components for Push Protocol products.

### 1. Add a component

Run the following command to add a component:

```bash
npx push-express add [component]
```

or

```bash
push-express add [component]
```

> **Note:** Replace `[component]` with the specific Push Protocol product you want to integrate (e.g., `notification`, `chat`, etc.).

### 2. Select the file type

After running the previous command, select the file type for your project:

- **TypeScript** (default)
- **JavaScript**

### 3. Install dependencies

After adding the component, **Push Express** will ask how you want to install the dependencies:

- **Yarn**: Automatically installs dependencies using Yarn.
- **NPM**: Automatically installs dependencies using NPM.
- **Manual**: It will display the command to install them manually.

```bash
npm install @pushprotocol/restapi@latest ethers@^5.7
```

### 4. Start your project

Once the component has been added and the dependencies are installed, you can start your project:

```bash
npm run dev
```

or

```bash
yarn dev
```

## Example

Here’s an example of what your project structure might look like after adding a component:

```bash
src/
├── components/
│   └── push-notification/
│       ├── index.ts
│       └── push-notification.tsx
└── service/
    └── push-notification/
        ├── index.ts
        └── push-notification.service.ts
```

## Contributions

Contributions are welcome! If you want to contribute to **Push Express**, follow these steps:

1. Fork the project [https://github.com/wolfcito/push-express](https://github.com/wolfcito/push-express).
2. Create a branch for your feature (`git checkout -b feature/new-feature`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature/new-feature`).
5. Open a pull request.

> ⚠️ **Warning**:  
> The code in this repository is provided without any warranties. It is important to note that the code has not been audited for potential security vulnerabilities. Using this code could result in fund loss, compromised data, or asset risks. Proceed with caution and use this code at your own risk. Please refer to the LICENSE file for more details on the terms and conditions.

## License

This project is licensed under the MIT license. For more information, check the [LICENSE](LICENSE) file.
