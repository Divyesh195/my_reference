# TailwindCSS 4.0

1. Add below code into global.css file and add scrollbar class to the component, of which you want to remove scrollbar.

```
.scrollbar::-webkit-scrollbar {
    width: 0px;
}
```

2. To make custom color variables add this code into global.css in next js project.


```
@theme {
  --color-lighthover: #fcf4ff;
  --color-darkhover : #2a004a;
  --color-darktheme : #11001f;
}
```

3. To apply images dynamically using map function, do not use bg-url class. Use this instead.

```
style={{ backgroundImage: `url(${items.img})` }}
```