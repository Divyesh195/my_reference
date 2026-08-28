# Next Js 15

## 1. Add following command in the next.config.js file to make "Pages" folder work. (App Router)

```
async rewrites() {
   return [
     {
       source: "/:path*",
       destination: "/Pages/:path*",
     },
   ];
},
```
## 2. Use of environment variables. 
First create a .env.local file in root directory. Then add variables with prefix "NEXT_PUBLIC"
```
NEXT_PUBLIC_SITE_URL = http://localhost:3000
```
Access this variables using this command 
```
process.env.NEXT_PUBLIC_SITE_URL
```

## 3. Next JS Upgrade
```
Change the Next js version in package.json file and run 'npm install' command.
```

## 4. Test production build
```
npm run build              # creates .next folder
npm run start             # starts production server
```
No auto‑reload; this mimics real deployment.