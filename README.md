I have a mono-repository with several small applications and libraries that have similar configurations and the same structure.

Usually, nowadays, when you bootstrap a project with Vite for instance, it generates 3-4 tsconfig.json.

- tsconfig.json // Have references to app, node, vitest tsconfig.json
- tsconfig.app.json // For the application files
- tsconfig.node.json // For the configuration files
- tsconfig.vitest.json // If you add vitest

So I wanted to leverage the usage of `${configDir}` to handle them in one place.

To illustrate a bit my explanation, I created a small dummy repository.

[Github](https://github.com/Lukinoh/configdir-example)
[Stackblitz](https://stackblitz.com/github//Lukinoh/configdir-example)
