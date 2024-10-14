> [!NOTE]
> This fork of [cps-elements](https://github.com/cpsrepositorio/cps-elements/) in my personal account is for giving more visibility to the project, especially to non Portuguese-speaking people, by offering this `README` in English. Anyway, contributions directly here are allowed, since both repos are synced often.

# CPS Elements

**Cutting-edge Web Components, hassle-free.**

- Components in the browser, without _frameworks_; 🌐
- And natively supported in _frameworks_ like [Vue](./docs/frameworks/vue) and [Angular](./docs/frameworks/angular); 🧩
- Or with included _wrappers_ to support [React](./docs/frameworks/react); ⚛️
- Packaged for direct access via [CDN](./docs/fundamentos/instalacao.md#atraves-de-cdn); 📦
- Fully compliant with the [CPS Design System](https://cpsrepositorio.github.io/cps-design-system/); 🎨
- Including a dark mode theme; 😎
- But fully customizable with CSS; 📝
- Built with accessibility in mind; ♿️
- In Portuguese, but supporting internationalization; 💬
- And completely _open-source_! 🔓

CPS Elements is part of an institutional UI/UX project for the ["Paula Souza" State Center for Technological Education](https://www.cps.sp.gov.br/), a São Paulo State governmental educational autarchy. The project is also composed of the CPS Design System, originally designed by Professor [Erick Petrucelli](https://github.com/ErickPetru). Regardless of its origins and initial motivations, it is a completely _open-source_ project available under the terms of the [MIT license](LICENSE.md).

---

Documentation: [cpsrepositorio.github.io/cps-elements](https://cpsrepositorio.github.io/cps-elements/)

Source code: [github.com/cpsrepositorio/cps-elements](https://github.com/cpsrepositorio/cps-elements/)

---

## What is this project about?

After a long time, we finally have a native way to create [our own HTML elements](https://developer.mozilla.org/docs/Web/Web_Components) and use them with any JavaScript _framework_ we want, or even without any _framework_! Although it is a native specification [with excellent support in modern browsers](https://caniuse.com/custom-elementsv1), building all the components from scratch, fitting properly and following best practices, is a costly action that many teams cannot take on (and shouldn't).

CPS Elements provides a collection of professionally designed components, created with framework-agnostic technology, adhering to the design established in the [CPS Design System](https://cpsrepositorio.github.io/cps-design-system/). Thus, you can start your projects without having to reinvent the wheel, based on a modern component library, directly in the browser (using only standard HTML and JavaScript), or along with your favorite _framework_, be it React, Vue, or Angular.

## How to run the source code?

If you are or want to be a contributor, you can use this documentation to understand how to build CPS Elements from the source code. You will need an environment running [Node](https://nodejs.org/en) from version `14.17`, to compile and run the project locally.

**You don't need to do any of this to use CPS Elements!** This page is aimed at people who want to contribute to the project, adjust its source code, or even build something new based on CPS Elements.

If this is not what you are trying to do, the [documentation](https://cpsrepositorio.github.io/cps-elements) is where you really want to be to get started with using the components.

### What are you using to build CPS Elements?

The components themselves are made with [LitElement](https://lit-element.polymer-project.org/), a base class for creating custom elements that offers an intuitive API and support for reactive data binding. The build package is then created through a custom build script, assembled with [esbuild](https://esbuild.github.io/).

The base is like that, but many other techniques and technologies are in use, such as CSS with _custom properties_ (variables), TypeScript, Iconify, Web Test Runner, ESLint, Prettier, among others. Browsing this repository for a while is the best way to observe everything that is in use to create this component library.

### Forking the repository

As is common in _open-source_ projects, start contributing by [creating your own fork](https://github.com/cpsrepositorio/cps-elements/fork) on GitHub, and then make a local clone, finally installing the dependencies.

```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/cps-elements
cd cps-elements
npm install
```

### Developing

Once the repository is cloned, run the command:

```bash
npm run dev
```

This will start the local development server for CPS Elements. After the initial build (which may take a bit longer than subsequent ones), your default browser will open automatically.

There is no _hot module reloading_ (HMR) feature in this project, as browsers do not offer a mechanism to re-register custom elements, so generally, after saving changes to the source code, your browser will reload the page completely to display the updated content.

The documentation for this project is written in Markdown and generated as a static site through Docsify, at runtime. Thus, there is no documentation build script, and it can be changed in real-time, which will also cause the browser to reload completely after a save.

### Building

To generate a production build, run the command:

```bash
npm run build
```

The production build can then be tested locally with:

```bash
npm start
```

### Creating new components

There is an NPM script available to generate the base for new components. To do this, run the following command, replacing `cps-tag-name` with the desired HTML tag name for the new component.

```bash
npm run create cps-tag-name
```

This will generate a source code `.ts` file, a styles file, and a documentation page for the new component. When you start the development server, you will automatically find the new component in the "Components" section of the sidebar.

### Contributing

Although an initiative originated as part of an internal UI/UX project, which also supports the CPS Design System, CPS Elements is an _open-source_ project, and contributions are encouraged! If you are interested in contributing, please first check the [contribution guidelines](CONTRIBUTING.md).

Any kind of support you offer will be greatly appreciated! 👇

- [Star the repository](https://github.com/cpsrepositorio/cps-elements/stargazers)
- [Fork to contribute](https://github.com/cpsrepositorio/cps-elements/fork)

## License

CPS Elements was initially designed by Professor [Erick Petrucelli](https://github.com/ErickPetru). It is available under the terms of the [MIT license](LICENSE.md).
