### TimeLine Verticle using css

`index.html`
```javascript
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <section class="timeline-area">
        <div>
            <h2>Full-Stack Developer</h2>
            <h3>Google</h3>
            <h4>2024 - 2025</h4>
        </div>
        <div>
            <h2>Back-End Developer</h2>
            <h3>Facebook</h3>
            <h4>2023 - 2024</h4>
        </div>
        <div>
            <h2>Front-End Developer</h2>
            <h3>Twitter</h3>
            <h4>2022 - 2023</h4>
        </div>
    </section>
</body>
</html>
```

---


`style.css`
```javascript
* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

body {
    background: #131f33;
}

.timeline-area {
    margin: 90px auto;
    width: 360px;
    padding: 0 20px 0 30px;
    border-left: 2px solid #ccc;
}

div {
    background: #fff;
    padding: 10px 25px;
    border: 1px solid #ccc;
    height: 110px;
    margin-bottom: 20px;
    position: relative;
}


div:before {
    content: '';
    display: block;
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background-color: #000;
    border: 3px solid #ddd;
    display: block;
    position: absolute;
    top: 10px;
    left: -40px;
}


div:after {
    content: '';
    width: 0;
    height: 0;
    border-style: solid;
    border-color: transparent #ddd transparent transparent;
    border-width: 8px;
    position: absolute;
    top: 10px;
    left: -17px;
}

```