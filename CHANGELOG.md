# Changelog


## v0.0.2


### 🚀 Enhancements

  - Add get-port library The get-port library is added to the project. This library provides a way to get an available port number for the application to listen on. The library provides a function called `getPort` which returns a promise that resolves to an available port number. The library also provides functions to check if a port is safe or unsafe, and to wait for a port to become available. The library is added to the project to make it easier to run the application on different ports and to avoid conflicts with other applications running on the same machine. The `.eslintignore`, `.eslintrc`, `.gitignore`, and `src/unsafe-ports.ts` files are also added to the project as part of this change. ([c40e893](https://github.com/nyxblabs/scotty-beam-me-up/commit/c40e893))

### 🏡 Chore

  - **.eslintrc): disable @next/next/no-html-link-for-pages rule and set React version to 18 ✅ test(index.test.ts, utils.ts:** Add tests for getPort function and create utility functions to block ports The @next/next/no-html-link-for-pages rule is disabled to allow the use of HTML links in Next.js pages. The React version is set to 18 to ensure compatibility with the latest version of React. Tests are added to ensure the getPort function works as expected. Utility functions are added to block ports for testing purposes. ([8f91ee3](https://github.com/nyxblabs/scotty-beam-me-up/commit/8f91ee3))
  - **.eslintignore): add README.md to ignored files 🎨 style(README.md): format README.md file 🚀 feat(README.md:** Add documentation for scotty-beam-me-up package The first commit adds README.md to the ignored files in the eslint configuration. The second commit formats the README.md file. The third commit adds documentation for the scotty-beam-me-up package, including usage instructions, options, and license information. ([2516d03](https://github.com/nyxblabs/scotty-beam-me-up/commit/2516d03))

### ❤️  Contributors

- Nyxb <contact@nyxb.xyz>

