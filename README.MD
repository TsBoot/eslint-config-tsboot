
# 使用方法

```cli
yarn add  -D eslint @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint-config-tsboot
```

```json
// 。eslintrc.json
{
    "env": {
        "browser": false,
        "node": true,
        "commonjs": true,
        "es2021": true
    },
    "extends": [
        "eslint:recommended",
        "plugin:@typescript-eslint/eslint-recommended",
        "plugin:@typescript-eslint/recommended",
        "tsboot"
    ],
    "parser": "@typescript-eslint/parser",
    "parserOptions": {
        "ecmaVersion": 12
    },
    "plugins": [
        "@typescript-eslint"
    ],
      "settings": {
        "import/resolver": {
          "node": {
            "extensions": [
              ".ts",
              ".js",
              ".json",
              ".node"
            ],
            "paths": [
              "src"
            ]
          }
        }
      }
}

```