# JavaScript编译器Babel

- [Docs](https://babeljs.io/docs/en/)

## 安装

```sh
npm install --save-dev @babel/core @babel/cli
```

package.json

```json
"scripts": {
  "watch": "babel src --out-dir lib --source-maps inline --watch",
  "build": "babel src --out-dir lib --source-maps inline"
},
```

## 环境预设

[Docs](https://babeljs.io/docs/en/babel-preset-env)

```sh
npm install --save-dev @babel/preset-env
```

.babelrc

```json
{
  "presets": [
    [
      "@babel/preset-env", {
        "targets": "> 0.25%, not dead"
      }
    ]
  ]
}
```