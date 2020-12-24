# Using Next.js with PNPM

## Create App

```sh
#apt or yum install libvips
pnpm init next-app <project-name>
cd <project-name>
rm -rf node_modules package-lock.json
pnpm i

pnpm dev
```

### Build SPA

add command:

```json
{
  "scripts": {
    "spa": "next build && next export"
  }
}
```

run command

```sh
pnpm out
```

use `./out` by [ran](https://github.com/m3ng9i/ran) or [serve](https://github.com/vercel/serve)

```
ran -r ./out
```
