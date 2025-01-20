# Follow this steps to configure Tailwind CSS environment

Step 1: Install Tailwind CSS 
>npm install -D tailwindcss
>npx tailwindcss init

Step 2 : Configure template paths in "tailwind.config.js" file.

Step 3 : Add derivatives into a ./src/input.css file. 
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

Step 4 : Start Tailwind CSS CLI build process
>npx tailwindcss -i ./src/input.css -o ./src/output.css --watch

Step 5 : Add output.css file in main HTML file.


