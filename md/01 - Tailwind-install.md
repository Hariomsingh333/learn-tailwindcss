# Date: 04 / 01 / 2022

# Install Tailwindcss

you can install Tailwind css different ways,

<br>

you can use:

- tailwind cli
- using postcss
- using framework like (next.js, Laravel, )

but we are using post css way.

Steps

- create index.html
- npm init
- install tailwindcss and other package
- create tailwind.css or yourname.css
- write your three tailwind layer to your css file
- create tailwindcss config and postcss config
- run the your script

   <br>

1. create index.html
   <br>
   fist you need to create index.html and write your simple boilerplate code

2. npm init
   <br>
   second you need to create package.json file using npm init tag

```bash
npm init -y
```

3. install tailwindcss and other package
   <br>
   once your package.json file crate then you need to install tailwindcss and other package

```bash
npm install -D tailwindcss postcss autoprefixer vite
```

4. create tailwind.css or yourname.css
   <br>
   then you need to create you css file

5. write your three tailwind layer to your css file
   <br>
   once your css file created then you need to write those three tailwind layer

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

6. create tailwindcss config and postcss config
   <br>
   create the tailwindcss config and postcss config using this command

```bash
npx tailwindcss init -p
```

```js
// tailwind.config.js
module.exports = {
  content: ["*"],
  theme: {
    extend: {},
  },
  plugins: [],
};
```

```js
// postcss.config.js
module.exports = {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  },
};
```

7. run the your script
   when all step are done then run your script command

```json
  "scripts": {
    "start": "vite"
  },
```
