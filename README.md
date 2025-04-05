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

1. **Catch more bugs at compile time**: Stricter type checking helps identify potential issues before your code runs.
2. **Improve code quality**: Enforcing stricter rules encourages better coding practices.
3. **Enhance developer experience**: Consistent type checking rules across projects makes it easier for developers to switch between codebases.
4. **Reduce runtime errors**: Many bugs that would only appear at runtime are caught during development.
5. **Better IDE support**: Stricter type checking enables better autocomplete and refactoring capabilities in your IDE.

## Enabled TypeScript Compiler Options

This configuration enables the following compiler options:

| Option                               | Description                                                                                                                                                    |
| ------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `isolatedModules`                    | Ensure that each file can be safely transpiled without relying on other imports.                                                                               |
| `verbatimModuleSyntax`               | Do not transform or elide any imports or exports not marked as type-only, ensuring they are written in the output file's format based on the 'module' setting. |
| `erasableSyntaxOnly`                 | Do not allow runtime constructs that are not part of ECMAScript.                                                                                               |
| `forceConsistentCasingInFileNames`   | Ensure that casing is correct in imports.                                                                                                                      |
| `strict`                             | Enable all strict type-checking options.                                                                                                                       |
| `noImplicitAny`                      | Enable error reporting for expressions and declarations with an implied 'any' type.                                                                            |
| `strictNullChecks`                   | When type checking, take into account 'null' and 'undefined'.                                                                                                  |
| `strictFunctionTypes`                | When assigning functions, check to ensure parameters and the return values are subtype-compatible.                                                             |
| `strictBindCallApply`                | Check that the arguments for 'bind', 'call', and 'apply' methods match the original function.                                                                  |
| `strictPropertyInitialization`       | Check for class properties that are declared but not set in the constructor.                                                                                   |
| `strictBuiltinIteratorReturn`        | Built-in iterators are instantiated with a 'TReturn' type of 'undefined' instead of 'any'.                                                                     |
| `noImplicitThis`                     | Enable error reporting when 'this' is given the type 'any'.                                                                                                    |
| `useUnknownInCatchVariables`         | Default catch clause variables as 'unknown' instead of 'any'.                                                                                                  |
| `alwaysStrict`                       | Ensure 'use strict' is always emitted.                                                                                                                         |
| `noUnusedLocals`                     | Enable error reporting when local variables aren't read.                                                                                                       |
| `noUnusedParameters`                 | Raise an error when a function parameter isn't read.                                                                                                           |
| `exactOptionalPropertyTypes`         | Interpret optional property types as written, rather than adding 'undefined'.                                                                                  |
| `noImplicitReturns`                  | Enable error reporting for codepaths that do not explicitly return in a function.                                                                              |
| `noFallthroughCasesInSwitch`         | Enable error reporting for fallthrough cases in switch statements.                                                                                             |
| `noUncheckedIndexedAccess`           | Add 'undefined' to a type when accessed using an index.                                                                                                        |
| `noImplicitOverride`                 | Ensure overriding members in derived classes are marked with an override modifier.                                                                             |
| `noPropertyAccessFromIndexSignature` | Enforces using indexed accessors for keys declared using an indexed type.                                                                                      |
| `allowUnusedLabels`                  | Disable error reporting for unused labels.                                                                                                                     |
| `allowUnreachableCode`               | Disable error reporting for unreachable code                                                                                                                   |

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
