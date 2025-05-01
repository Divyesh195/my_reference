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
