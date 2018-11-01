Minimal vanilla js lightbox for images

[**Live example**](https://kormyen.github.io/lightbox/index.html)

<img src='PREVIEW.gif'/>
<img src='PREVIEW.jpg'/>

### Other Examples

- [Memex](https://kormyen.github.io/memex/) - [repo](https://github.com/kormyen/memex)
- [Shinestrength's Portfolio](http://www.shinestrength.xyz/) - [repo](https://github.com/shinestrength/memex)

#### Use

```
<head>
  <link rel="stylesheet" href="lightbox.css">
</head>
<body>
  <div class="lightbox"></div>
  <img src="image.jpg" onclick="lightbox.load('image.jpg')">
  <script src="lightbox.js"></script>
  <script>
    let lightbox = new Lightbox();
    lightbox.install(document.querySelector('.lightbox'), 'lightbox');
  </script>
</body>
```

#### Install
| install param | description                                      |
|          ---: | :---                                             |
|     container | containing div for lightbox to use               |
|        prefix | css class name prefix for 'x-img' and 'x-back'   |

#### Load
```
let image = document.querySelector(".image");
image.addEventListener('click', function(){ lightbox.load('image.jpg') });
```
or
```
<img src="image.jpg" onclick="lightbox.load('image.jpg')">
```