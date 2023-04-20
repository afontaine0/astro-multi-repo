# Astro Starter Kit: Basics

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   └── Card.astro
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       ├── index.astro
│       ├── _modules/
│       │   └── astro-multi-repo-content/
│       │       └── get-started.mdx
│       └── docs/
│           └── some-package/->../_modules/astro-multi-repo-content/
└── package.json
```

[`src/pages/_modules/astro-multi-repo-content`](./src/pages/_modules/astro-multi-repo-content) is a Git Submodule pointing to [afontaine0/astro-multi-repo-content](https://github.com/afontaine0/astro-multi-repo-content/tree/main).

[`src/pages/docs/some-package`](./src/pages/docs/some-package) is a symlink pointing to [`src/pages/_modules/astro-multi-repo-content`](./src/pages/_modules/astro-multi-repo-content). Therefore, the file [`get-started.mdx`](https://github.com/afontaine0/astro-multi-repo-content/blob/main/get-started.mdx) of the [afontaine0/astro-multi-repo-content](https://github.com/afontaine0/astro-multi-repo-content/tree/main) repository is directly available at [http://127.0.0.1:3000/docs/some-package/get-started](http://127.0.0.1:3000/docs/some-package/get-started).

The URL [http://127.0.0.1:3000/docs/_modules/astro-multi-repo-content/get-started](http://127.0.0.1:3000/docs/_modules/astro-multi-repo-content/get-started) will not be available because [Astro does not build pages prefixed by an underscore](https://docs.astro.build/en/core-concepts/routing/#:~:text=You%20can%20exclude%20pages%20or%20directories%20from%20being%20built%20by%20prefixing%20their%20names%20with%20an%20underscore%20(_).).

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                | Action                                           |
| :--------------------- | :----------------------------------------------- |
| `npm install`          | Installs dependencies                            |
| `npm run dev`          | Starts local dev server at `localhost:3000`      |
| `npm run build`        | Build your production site to `./dist/`          |
| `npm run preview`      | Preview your build locally, before deploying     |
| `npm run astro ...`    | Run CLI commands like `astro add`, `astro check` |
| `npm run astro --help` | Get help using the Astro CLI                     |

