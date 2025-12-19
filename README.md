# Config Library

Shared configuration library for ESLint, Prettier, and TypeScript projects.

## Installation

```bash
npm install --save-dev @c00lc4t775/config-lib
```

## Usage

### ESLint

Create or update your `eslint.config.js`:

```javascript
import configLib from '@c00lc4t775/config-lib/eslint.config.js';

export default configLib;
```

Or extend it:

```javascript
import configLib from '@c00lc4t775/config-lib/eslint.config.js';

export default [
  ...configLib,
  // your custom rules
];
```

### Prettier

Create or update your `prettier.config.js`:

```javascript
import configLib from '@c00lc4t775/config-lib/prettier.config.js';

export default configLib;
```

### TypeScript

Extend the base TypeScript configuration in your `tsconfig.json`:

```json
{
  "extends": "@c00lc4t775/config-lib/tsconfig.json",
  "compilerOptions": {
    // your custom options
  }
}
```

For app-specific configuration:

```json
{
  "extends": "@c00lc4t775/config-lib/tsconfig.app.json",
  "compilerOptions": {
    // your custom options
  }
}
```

For Node.js specific configuration:

```json
{
  "extends": "@c00lc4t775/config-lib/tsconfig.node.json",
  "compilerOptions": {
    // your custom options
  }
}
```

## Available Configurations

- `eslint.config.js` - ESLint configuration for React + TypeScript projects
- `prettier.config.js` - Prettier configuration
- `tsconfig.json` - Base TypeScript configuration
- `tsconfig.app.json` - TypeScript configuration for application code
- `tsconfig.node.json` - TypeScript configuration for Node.js/build tools

