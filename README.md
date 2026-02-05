## Safirial Icons – SVG Icon Package (Universal)

**Safirial Icons** is an SVG icon package compatible with Angular, React, Vue, and vanilla JavaScript/TypeScript projects.  
It provides a list of icon names and a function to resolve static paths to SVGs.

This package can be used standalone or alongside the `catarina` design system.

- **npm package**: `safirial-icons`
- **Version**: `1.0.3`

---

## Public API

The `index.ts` file exposes the following elements:

- `ICON_BASE_PATH`: base path where SVGs are served (`'safirial-icons'`).
- `iconList`: list of available icon names (e.g., `'home'`, `'sun'`, `'email'`, `'github'`, etc.).
- `IconName`: TypeScript type representing any valid icon name.
- `getIconPath(name: IconName): string`: function that returns the complete SVG path from the name.

Example of direct usage of `getIconPath`:

```ts
import { getIconPath, IconName } from 'safirial-icons';

const iconName: IconName = 'home';
const path = getIconPath(iconName); // 'safirial-icons/home.svg'
```

## Installation

In any project (Angular, React, Vue, or vanilla JavaScript/TypeScript):

```bash
npm install safirial-icons
```

It can also be installed using `pnpm` or `yarn`:

```bash
pnpm add safirial-icons
yarn add safirial-icons
```

## Building and publishing

To compile the library:

```bash
npm run build
```

The output is generated in:

```bash
dist/
```

This will compile TypeScript to JavaScript and copy SVG assets to the `dist` folder.

---

## Credits and attribution

The SVG icons included in this package come from the following sources:

### Heroicons

Icons are based on [Heroicons](https://heroicons.com/outline), created by the developers of Tailwind CSS.

- **Website**: [https://heroicons.com/outline](https://heroicons.com/outline)
- **License**: MIT License
- **Version**: v2.1.5

### SVG Repo

Some additional icons come from [SVG Repo](https://www.svgrepo.com/), an open-source SVG icon collection.

- **Website**: [https://www.svgrepo.com/](https://www.svgrepo.com/)
- **Licenses**: Various (MIT, Apache 2.0, CC0)

All icons retain their original licenses as applicable. Attribution is maintained in accordance with the respective license terms.

---

## Language / Idioma

This documentation is available in English. For the Spanish version, see [README.es.md](./README.es.md).

Esta documentación está disponible en inglés. Para la versión en español, consulta [README.es.md](./README.es.md).

---