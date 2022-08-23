# Dark-Light-mode-Tailwindcss-example
![light](/prz/light%20prz.png)
![dark](/prz/dark%20prz.png)

#1 Install Tailwind CSS:
```
npm install -D tailwindcss
npx tailwindcss init
```
#2 Configure your template paths:\
```
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

#3 Add the Tailwind directives to your CSS:
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```
#4 Start the Tailwind CLI build process:
```
npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```
#5 add a script to run css updates :
```
"scripts": {
    "build:css": "tailwindcss -i ./src/input.css -o dist/output.css --watch"
  }

script in terminal: npm run build.css 

```