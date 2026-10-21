# @rho-softwares/cljsdt-toolchain

The tools a [cljsdt](https://github.com/rho-softwares/cljsdt) project runs, in one dependency:

- **Idris 2** 0.8.0 on Chez Scheme 10.4.1, relocatable: the verifier (`@cljsdt/idris2-linux-x64`; BSD-3-Clause and Apache-2.0, licenses inside)
- **clj-kondo**: the linter (`@cljsdt/clj-kondo-linux-x64`; EPL-1.0)
- **esbuild**: `cljsdt build --script` puts what a program uses of its JS libraries in its one file (MIT)
- **shadow-cljs**: `cljsdt build --browser` (not available yet in 0.1)

`npx cljsdt create my-app` puts it in the new project. In an existing project:

```sh
npm i -D cljsdt @rho-softwares/cljsdt-toolchain
```

Linux x64 for now. This package has no code of its own (MIT); each tool keeps its license.
