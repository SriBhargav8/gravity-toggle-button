# gravity-toggle-button

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gravity Toggle Button</title>
    <link rel="stylesheet" href="/stylesheet.css">
    <style>
        body{
    margin: 0;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #f2f2f2;
}

input[type='checkbox']{
    -webkit-appearance: none;
    width: 250px;
    height: 100px;
    outline: none;
    border: 2px solid black;
    border-radius: 50px;
    background-color: #fff;
    cursor: pointer;
    box-shadow: 0px 10px 20px rgba(0, 0, 0, 3);
    transition: all 0.3s;
    position: relative;
}
input[type='checkbox']::before{
    content: '';
    position: absolute;
    width: 100px;
    height: 100%;
    border: 2px solid black;
    border-radius: 50% ;
    left: 0;
    top: 50%;
    transform: translateY(-50%) scale(0.9);
    background-color: orange;
    transition: all 0.3s;
    box-sizing: border-box;
}
input[type='checkbox']:checked{
    background-color: orange;
    transform: rotate(90deg);
}
input[type='checkbox']:checked:before{
    left: calc(100% - 100px);
    background-color: #fff;
    transition: left 0.6s cubic-bezier(0.9, 0.05, 0.7, 0.19) 0.2s;
}
    </style>
     
</head>
<body>
  <input type="checkbox">
</body>
</html>
