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