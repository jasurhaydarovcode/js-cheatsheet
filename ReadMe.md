<h1 align="center">Java Script Components by <a href="https://github.com/jasurbekhaydarovcode">JASURBEK HAYDAROV</a></h1>


# Components
---
## № 1 , Site Loading
- ### If you type any element class name in this code it will disappear with in 2 seconds
```js
document.addEventListener("DOMContentLoaded", function() {
    setTimeout(function() {
        var element = document.querySelector('.className');
        if (element) {
            element.remove();
        }
    }, 2000); // 2 second in remove
});
```

---

## № 2 , Onclick Size Change

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Onclick() Size</title>
</head>

<body>
    <style>
        body {
            font-family: sans-serif;
        }

        h1,
        p {
            text-align: center;
        }
    </style>

    <div>
        <p id="paragraph">Some paragraph text</p>
        <h1 id="heading1">some heading 1 text</h>
            <h1 id="heading2">some heading 2 text</h1>
    </div>
    <div class="buttons">
        <button onclick="changeFontSize(12)">12</button>
        <button onclick="changeFontSize(24)">24</button>
        <button onclick="changeFontSize(46)">46</button>
    </div>

    <script src="size.js"></script>
    <script>
        function changeFontSize(size) {
            document.querySelector('#paragraph').style.fontSize = size + 'px';
            document.querySelector('#heading1').style.fontSize = size + 'px';
            document.querySelector('#heading2').style.fontSize = size + 'px';
        }
    </script>
</body>

</html>
```