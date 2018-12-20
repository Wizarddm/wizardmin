# Using TypeScript with React Native

## Adding TypeScript

The next step is to add TypeScript to your project. The following commands will:

+ add TypeScript to your project
+ add React Native TypeScript Transformer to your project
+ initialize an empty TypeScript config file, which we'll configure next
+ add an empty React Native TypeScript Transformer config file, which we'll configure next
+ adds typings for React and React Native

Okay, let's go ahead and run these.

```shell
yarn add --dev typescript
yarn add --dev react-native-typescript-transformer
yarn tsc --init --pretty --jsx react
touch rn-cli.config.js
yarn add --dev @types/react @types/react-native
```

The rn-cli.config.js contains the settings for the React Native TypeScript Transformer. Open it and add the following:

```javascript
module.exports = {
  getTransformModulePath() {
    return require.resolve('react-native-typescript-transformer');
  },
  getSourceExts() {
    return ['ts', 'tsx'];
  },
};
```

## Migrating to TypeScript

Rename the generated App.js and __tests_/App.js files to App.tsx. index.js needs to use the .js extension. All new files should use the .tsx extension (or .ts if the file doesn't contain any JSX).

If you tried to run the app now, you'd get an error like object prototype may only be an object or null. This is caused by a failure to import the default export from React as well as a named export on the same line. Open App.tsx and modify the import at the top of the file:

```javascript
-import React, { Component } from 'react';
+import React from 'react'
+import { Component } from 'react';
```