# Next Js 15

1. Add following command in the next.config.js file to make "Pages" folder work. (App Router)

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
2. To create Next js app using PNPM use this command
```
pnpm create next-app
```
3. To use environment variables in local machine.
```
First create a .env.local file in root directory. Then add variables with prefix NEXT_PUBLIC
Exmaple : NEXT_PUBLIC_SITE_URL = http://localhost:3000

Access this variables using this command : process.env.NEXT_PUBLIC_SITE_URL
```