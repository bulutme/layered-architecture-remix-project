# Akakçe Remix Case Study!

- [Remix Docs](https://remix.run/docs)

## Env

Create .env file at root

```sh
API_PRODUCTS_URL=<product-list-api-url>
```

```sh
API_SINGLE_PRODUCT_URL=<single-product-list-api-url>
```

## Development

From your terminal:

```sh
npm run dev
```

This starts your app in development mode, rebuilding assets on file changes.

## Test

All test cases will be running, you can check console

```sh
npm run test
```

## Deployment

First, build your app for production:

```sh
npm run build
```

Then run the app in production mode:

```sh
npm start
```

Now you'll need to pick a host to deploy it to.

### DIY

If you're familiar with deploying node applications, the built-in Remix app server is production-ready.

Make sure to deploy the output of `remix build`

- `build/`
- `public/build/`

### Using a Template

When you ran `npx create-remix@latest` there were a few choices for hosting. You can run that again to create a new project, then copy over your `app/` folder to the new project that's pre-configured for your target server.

```sh
cd ..
# create a new project, and pick a pre-configured host
npx create-remix@latest
cd my-new-remix-app
# remove the new project's app (not the old one!)
rm -rf app
# copy your app over
cp -R ../my-old-remix-app/app app
```

That project is built according to Clean Arthitecture and SOLID principles.

Single Responsibility Principle (SRP)  
Open Closed Principle (OCP).  
Liskov Substitution Principle (LSP).  
Interface Segregation Principle (ISP).  
Dependency Inversion Principle (DIP)  
Separation of Concerns (SOC).  
Don't Repeat Yourself (DRY)
