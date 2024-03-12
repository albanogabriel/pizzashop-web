# SHADCN / UI
https://ui.shadcn.com/docs/installation/vite
  
->  npm install -D tailwindcss postcss autoprefixer
->  npx tailwindcss init -p
  
-> Edit tsconfig.json file 
>  ts.config: abaixo do compilerOptions
      "baseUrl": ".",
      "paths": {
        "@/*": [
          "./src/*"
        ]
      }

->  npm i -D @types/node

>   vite.config.ts

    import path from "node:path"
    import { defineConfig } from 'vite'
    import react from '@vitejs/plugin-react'

    // https://vitejs.dev/config/
    export default defineConfig({
      plugins: [react()],
      resolve: {
        alias: {
          "@": path.resolve(__dirname, "./src"),
        },
      },
    })

->  npx shadcn-ui@latest init

    Need to install the following packages:
    shadcn-ui@0.8.0
    Ok to proceed? (y) 
    ✔ Would you like to use TypeScript (recommended)? … / yes
    ✔ Which style would you like to use? › Default
    ✔ Which color would you like to use as base color? › Zinc
    ✔ Where is your global CSS file? … src/global.css
    ✔ Would you like to use CSS variables for colors? … / yes
    ✔ Are you using a custom tailwind prefix eg. tw-? (Leave blank if not) … / space, leaved blank
    ✔ Where is your tailwind.config.js located? … tailwind.config.js
    ✔ Configure the import alias for components: … @/components
    ✔ Configure the import alias for utils: … @/lib/utils
    ✔ Are you using React Server Components? … no / yes
    ✔ Write configuration to components.json. Proceed? … yes

    ✔ Writing components.json...
    ✔ Initializing project...
    ✔ Installing dependencies...



