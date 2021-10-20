<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: consolas;
}

body{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background: #121213;
}
.loader{
    position: relative;
    -webkit-box-reflect: below 2px linear-gradient(transparent,#0002);
}

.loader::before{
    content: '';
    position: absolute;
    top: 0;
    right: 0;
    width: 2px;
    height: 100%;
    background: #d803f4;
    animation: blinkCursor 0.8s steps(3) infinite;
}
@keyframes blinkCursor {
    0%,75%
    {
        opacity: 1;
    }
    76%,100%
    {
        opacity: 0;
    }
}

.loader h2{
    position: relative;
    color: #d803f4;
    letter-spacing: 5px;
    font-size: 4em;
    text-transform: uppercase;
    animation: typing 8s steps(11) infinite ;
    overflow: hidden;
}
@keyframes typing {
    0%
    {
        width: 0;
    }
    30%,60%
    {
        width: 442.063px;
    }
}
/* //#03e9f4 */
        </style>
</head>
<body>
    <div class="loader">
        <h2>Hi_There...</h2>
    </div>
</body>
</html>
