## DNB Hugo Libs / Bootstrap 5

### Introduction

This is a Hugo theme component adding Bootstrap 5. It also imports [popper.js](https://github.com/dnb-hugo/libraries/tree/main/popper.js). It mounts the following directories:

-   `assets/libs/bootstrap/scss` to Bootstraps `scss` directory
-   `assets/libs/bootstrap/dist` to Bootstraps `dist` directory
-   `assets/vendor/_rfs.scss` to `_rfs.scss`, a vendor requirement for compiling Bootstrap via SASS
-   `assets/libs/popper.js` to the popper.js `src` directory (see [popper.js module documentation](https://github.com/dnb-hugo/libraries/tree/main/popper.js) on how to use)

### Installing

Step 1: Make sure that modules are enabled in your own repository. If there is no `go.mod` in your root directory run the following command and use a descriptive name. Typically, the repository-path without protocol in the beginning serves this purpose.

```shell script
hugo mod init github.com/username/reponame
```

Step 2: add the module to your required modules in `config.toml` or `config/module.toml`

```toml
[module]
[[module.imports]]
path = "github.com/dnb-hugo/libraries/bootstrap5"
```

The next time you run hugo it will download the latest version of the module.

### Versions

If you require explicit versions of Bootstrap here are the accompanying versions:

-   Bootstrap v5.0.0-beta2 - @dnb-hugo-libraries/bootstrap5 v1.3.0+
-   Bootstrap v5.0.0-beta1 - @dnb-hugo-libraries/bootstrap5 v1.2.0+

### Other libraries in DNB Hugo Libraries

-   [Bootstrap Icons](https://github.com/dnb-hugo/libraries/tree/main/bootstrap-icons)
-   [Bootstrap 5](https://github.com/dnb-hugo/libraries/tree/main/bootstrap5)
-   [Popper.js](https://github.com/dnb-hugo/libraries/tree/main/popper.js)

### Other elements in DNB Hugo

[DNB Hugo](https://github.com/dnb-hugo) are the elements that enhance and simplify your daily work with [Hugo, the world's fastest framework for building websites](https://gohugo.io/). Included are:

| Element | Description |
| :--- | :--- |
| [blocks](https://github.com/dnb-hugo/blocks) | Blocks are reusable page elements like headers, footers, content display etc.|
| [components](https://github.com/dnb-hugo/components) | Components are preconfigured features like automatic search index creation, sitemap and robots.txt creation, etc. |
| [libraries](https://github.com/dnb-hugo/libraries) | Libraries are a collection of often used external packages, conveniently configured as modules for Hugo. |
| [shortcodes](https://github.com/dnb-hugo/shortcodes) | Shortcodes are content particles that helpfully solve repeated tasks, like presentation, galleries and so on. |
| [testcontent](https://github.com/dnb-hugo/testcontent) | Testcontent is a collection of testing content. Obviously. |
