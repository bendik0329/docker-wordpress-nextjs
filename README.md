# contentful-shopify-app

## Getting Started

To run this locally make sure you have the following:

- Docker (with Compose)
- Yarn

To run it for first time:

```bash
yarn prepare && yarn start
```

Later you can run it without prepare:

```bash
yarn start
```

Visit the app at [http://localhost:3000](http://localhost:3000).  
Explore the api at [http://localhost:4000](http://localhost:4000).

## Deployment

To create the app:

```bash
doctl apps create --spec .do/production.yaml
```

To list running apps:

```bash
doctl apps list --format ID,Spec.Name
```

To update running app

```bash
doctl apps update <app-id> --spec .do/production.yaml
```
