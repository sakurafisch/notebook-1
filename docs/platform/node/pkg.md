# PKG

Server-side JS打包工具。

- 并不是所有的Node版本都可以打包的，这跟<https://github.com/zeit/pkg-fetch/releases>中的版本有关。
- 一般只有主版本号为偶数的版本适合打包。
- 变更版本号后，要重新安装`sqlite3`等原生依赖。

```sh
yarn global add pkg

pkg . # 等价于 `pkg package.json`
# pkg . --targets latest-win-x64

# 注意使用pkg能够处理的相应的Node版本，当涉及需要编译的二进制包时尤其如此。
# 另一种 pkg lib/index.js --targets latest
```
