# Welcome to MonoRepo!

- In a nutshell, monorepo is a strategy where you will have all the application’s code in the same repository.
- There are some cases that a monorepo fits well. For example, when you have an application with a mobile app, backend, frontend, and so on. With monorepo, we will have a folder for each of these parts and share code between them.
- With monorepo, you can have unique versions for each module as well.

## # Three Main Benefits

1. **♻️ Ease of code reuse** — When we have a project with many modules, but with the same codebase, it is good to have all these modules altogether in a monorepo. For example, an SDK that has a package for different frameworks’ components.
2. **📦 Simplified dependency management** — In a multiple repository environment where many projects depend on a third-party dependency, that dependency might be downloaded or built many times. In a monorepo, the build can be easily optimized, as referenced dependencies all exist in the same codebase. You can achieve it using Yarn Workspaces.
3. **🚀 Unified versioning** — We have one source of truth for all packages. It’s a good practice when you have an API with sub-modules, it will allow you to identify whether the module you are using came from the same codebase. For example, when a new version of core package is published, all “sub-packages” will have the same version.

> **Note**: remove all `node_modules` folders inside the packages and then run `yarn install` in the root folder. It will install the dependencies for all packages.
> For Better Understanding follow this article [here](https://medium.com/swlh/creating-testing-and-building-a-monorepo-with-lerna-and-yarn-1ced540e04c7).
