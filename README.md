# ec-vip-vue 隱形賣場

改善原先在 MVC 裡的 jQuery 架構，前後端分離有效提昇開發效率。

## Tech Stack

| **Package** | **Version** |
| ----------- | ----------- |
| Node.js     | v18.16.0    |
| yarn        | v1.22.21    |
| TypeScript  | v4.8.4      |
| Vue         | v3.2.41     |
| Vue Router  | v4.1.5      |
| Pinia       | v2.0.23     |
| Vite        | v3.1.8      |
| Vitest      | v0.34.6     |

## Screenshots

### 首頁 Index
![index](https://github.com/MollyLin/vue3-vip-mart/assets/7385444/c3257414-4dc1-4313-9775-439661558f20)

### Product detail Modal
![open-product-modal](https://github.com/MollyLin/vue3-vip-mart/assets/7385444/ac8a652a-51fc-4e62-b697-221cd2431ef6)

### 權限驗證 Passcode
![passcode](https://github.com/MollyLin/vue3-vip-mart/assets/7385444/2ec641d9-968f-4bf5-8739-fdf52957f998)

### Vitest UI
![網頁擷取_20-12-2023_15250_localhost](https://github.com/MollyLin/vue3-vip-mart/assets/7385444/af313c4b-d183-4e80-80a4-a3bc4b923a71)


## How I use it?

### STEP1: Swagger and local API Setup

```sh
yarn install
yarn run api
```

API address:
`http://localhost:3000/${api path}`

### STEP2: Project Setup

```sh
yarn run dev
```

Run the Project and access at:

- `http://localhost:5173/activity/活動代號`
- `http://localhost:5173/passcode/活動代號`

### Type-Check, Lint with [ESLint](https://eslint.org/)

```sh
yarn run type-check
yarn run format
yarn run lint
```

### Run Unit Tests with [Vitest](https://vitest.dev/)

```sh
yarn run test:unit
yarn run test:coverage
yarn run test:ui
```

### Run dependency cruiser

```shell
yarn add -D dependency-cruiser
npx depcruise --init
# src > no > yes > tsconfig.json > yes
npx depcruise src --include-only "^src" --output-type dot | dot -T svg > dependency-graph.svg
```

![visualise dependencies SVG](screenshots/dependency-graph.svg)
