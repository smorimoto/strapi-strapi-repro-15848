# strapi-strapi-repro-15848

## Creating the universe

```sh
git clone git@github.com:smorimoto/strapi-strapi-repro-15848.git
cd strapi-strapi-repro-15848
# Check out ca42ccb56e765f88c311635e2dee3d8a393da803 (4.6.1)
yarn install --immutable
# Create the universe with turborepo, but you can also use the @yarnpkg/plugin-workspace-tools instead
yarn build
# --------------- The error logs are expected to output here... ----------------
# Destroy the universe!!
rm -rf .yarn/cache node_modules
# Check out 758802315a0f46f4a02e92412af3104c15c92aa3 (0.0.0-9b5c6cf2e3db7f6a0227f25928c2dddcda9829f4)
yarn install --immutable
# Create the universe...
yarn build
# -------------- The successful logs are expected to output here! --------------
```
