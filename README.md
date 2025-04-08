# @allindevelopers/tsconfig

A shareable TypeScript configuration package that provides strict type checking rules to improve code quality and prevent common errors in your TypeScript projects.

## Purpose

This package provides a standardized, strict TypeScript configuration that can be used across multiple projects to ensure consistent type checking and code quality. It enables all the recommended strict type checking options to catch more potential issues at compile time.

## Installation

```bash
npm install --save-dev @allindevelopers/tsconfig
```

## Usage

You can extend this configuration in your project's `tsconfig.json`:

```json
{
	"extends": "@allindevelopers/tsconfig/strict.json",
	"compilerOptions": {
		// Your project-specific compiler options here
	},
	"include": ["src/**/*"],
	"exclude": ["node_modules", "dist"]
}
```

## Benefits of Strict Configuration

Using this strict TypeScript configuration provides several benefits:

1.  **Catch more bugs at compile time**: Stricter type checking helps identify potential issues before your code runs.
2.  **Improve code quality**: Enforcing stricter rules encourages better coding practices.
3.  **Enhance developer experience**: Consistent type checking rules across projects makes it easier for developers to switch between codebases.
4.  **Reduce runtime errors**: Many bugs that would only appear at runtime are caught during development.
5.  **Better IDE support**: Stricter type checking enables better autocomplete and refactoring capabilities in your IDE. |

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.

## Author

Andrei Luca (https://luca.md)

## Contributing

Contributions are welcome! If you'd like to contribute:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

Please make sure to update tests as appropriate and adhere to the project's code style.
