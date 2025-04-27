# Css
Learning css
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nav container</title>
</head>
<style>
    body{
        font-family: Arial, Helvetica, sans-serif,
        sans-serif;
        margin :0;
        padding :20px;
        background-color: black;
        color: whitesmoke;


    }
    .nav-container{
        margin-bottom: 40px;
    }
    h2{
        margin-bottom: 10px;
    }
    .nav1{
            background-color: #f8f9fa;
            padding:10px;
    }
    .nav1 ul {
        list-style-type: none;
        margin: 0%;
        padding: 0%;
        display: flex;
        justify-content: space-between;
        
    }
            .nav1 li{
                display: inline;
            }
            .nav1 a {
                text-decoration: none;
                color: rgb(223, 216, 217);
                background-color: rgb(121, 96, 31); 
                padding: 5px 10px;
                position: relative;
            }
            .nav1 a::after{
                content: "";
                position :absolute;
                height:2px;
                width:60px;
                bottom: 0;
                left: 0;
                background-color: #0e1e2e;
                transform: scaleX(0);
                transition: transform 0.3s ease-in-out;
            }
            .nav1 a:hover::after{
                transform: scaleX(1);
            }

            .nav1 .login-btn{
                background-color: #0e1e2e;
                color: aliceblue;
                border: none;
                padding: 5px 15px;
                border-radius: 5px;
                cursor: crosshair;
            }
</style>
<body>
    <div class="nav-container"><h2>
        Variation 1 :Horizontal with underline effeccrs
    </h2>
    <nav class="nav1">
        <ul>
            <li><a href ='#'>HOMe</a></li>
            <li><a href ='#'>About</a></li>
            <li><a href ='#' > products</a></li>
            <li><button class="login-btn">login</button></li>
        </ul>
    </nav>
</div>

    
</body>
</html>
