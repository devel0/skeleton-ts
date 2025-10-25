# skeleton-ts

## quickstart

```sh
mkdir skeleton-ts
cd skeleton-ts

curl https://raw.githubusercontent.com/github/gitignore/refs/heads/main/Node.gitignore > .gitignore

pnpm init
mkdir src dist
pnpm i typescript -D
npx tsc --init
echo "console.log('Hello, TypeScript!');" > src/index.ts
code .
```

- edit `tsconfig.json` uncommenting `rootDir` and `outDir`

- edit `package.json` adding following scripts

```json
{
    "scripts": {
        "build": "tsc",
        "start": "tsc && node dist/index.js",
    }
}
```

- from vscode C-S-p `Debug: Add Configuration...`
  - choose `More Node.js options...` 
  - then choose `Run Script: start`

- place a breakpoint into index.ts ( `F9` )

- hit `F5` to start debugger