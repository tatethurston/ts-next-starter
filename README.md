### Patch Shopify App

## Getting Started

Run the development server:

```bash
yarn start
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Tech stack

1. [Typescript](https://www.typescriptlang.org/docs/)
1. [React](https://reactjs.org/docs/getting-started.html)
1. [Next.js](https://nextjs.org/docs)
1. [SWR](https://swr.vercel.app/)
1. [Styled Components](https://styled-components.com/docs)

The `eslint` config comes from [eslint-config-react-app](https://github.com/facebook/create-react-app/tree/master/packages/eslint-config-react-app).

### Reasoning

Typescript was chosen to minimize development errors and eliminate the need for certain classes of tests. Especially when paired with a declarative framework like React, unit tests a few E2E / System tests will be sufficient.

Next.js was chosen over Create React App for it's strong performance characteristics, opinionated structure, and to minimize direct dependencies. Next supports prefetching, preloading, dynamic imports and static HTML exports out of the box. The opinionated page system establishes a nice patter that makes it easier for new developers to orient themselves and enforces reasonable architectural guard rails.

## Development

The `yarn lint:fix` command can be run to run `eslint` and `prettier` on the `src` directory. This command is automatically run as a pre-commit hook.

The `yarn build` command will create a static export with prerendered HTML. This can be served from S3, a web server, etc. You can serve this locally with the `yarn serve` command. Open [http://localhost:5000](http://localhost:5000) with your browser to see the result.
