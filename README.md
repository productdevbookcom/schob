# Schob

![Schob](https://github.com/productdevbookcom/schob/blob/main/.github/assets/schob.png?raw=true)


## Installation

```bash
pnpm add schob
```

## Usage

```ts
import { merge } from 'schob'

const schema = {
  isPro: false,
  darkMode: false,
  pages: {
    home: false,
    settings: false,
  },
}

const newData = {
  isPro: false,
  darkMode: true,
  pages: {
    home: false,
    settings: true,
    hello: false,
  },
  dd: 'dd',
  tt: {
    dd: 'dd',
  },
  cc: [{ dd: 'dd' }],
}

const res = merge({ schema, newData })
```

### Output
```bash

{
    isPro: false,
    darkMode: true,
    pages: { home: false, settings: true },
 }
 ```

## Sponsors

<p align="center">
  <a href="https://cdn.jsdelivr.net/gh/oku-ui/static/sponsors/sponsors.svg">
    <img alt="sponsors" src='https://cdn.jsdelivr.net/gh/oku-ui/static/sponsors/sponsors.svg'/>
  </a>
</p>


## License

MIT License © 2022-PRESENT [productdevbook](https://github.com/productdevbook)
