<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>Document Title</title>
    <link rel="stylesheet" href=".css">
    <link href="https://fonts.googleapis.com/css?family=Roboto:100,100italic,300,300italic,regular,italic,500,500italic,700,700italic,900,900italic" rel="stylesheet" />

<style>
    .box2 {
    background-image: radial-gradient(circle, rgb(0, 0, 0) , rgb(143, 143, 144) );
    width: 400px; /* Larger size */
    height: 400px; /* Larger size */
    display: inline-block;
    position: absolute;
    top: 0;
    left: 0;
    border-radius: 50%; /* Circular shape */
    animation: moveBigBubble 40s infinite;
    opacity: 0.1; /* Adjusted opacity */
}

@keyframes moveBigBubble {
    0% {
        top: 0;
        left: 0;
        border-radius: 44% 56% 74% 26% / 61% 64% 36% 39% ; /* Circular shape at start */
        transform: rotate(-50deg);

    }
    25%{
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        border-radius: 75% 25% 74% 26% / 61% 73% 27% 39% ; /* Change shape */

    }
    50% {
        top: 80%;
        left: 20%;
        transform: translate(-80%, -80%);
        border-radius: 28% 72% 93% 7% / 17% 73% 27% 83% ; /* Change shape */
       
    }
    75% { top: 80%;
        left: 0;
        transform: translate(-70%, -80%);

        border-radius: 66% 34% 21% 79% / 70% 73% 27% 30% ; /* Circular shape at end */
    }
       
    
    100% { 
        
        top: 0;
        left: 0;
        transform: rotate(-50deg);
        border-radius: 44% 56% 74% 26% / 61% 64% 36% 39%; /* Circular shape at end */
       
    }
}
    .body{
        height: 300px;
        width: 300px;
        background-image: radial-gradient(circle, rgb(11, 0, 14) , rgb(56, 10, 96) );
        background-repeat: no-repeat;
        height: 590px;
        
    }   

    .log {
    display: inline-block;
    position: relative;
    color: white;
    font-size: 40px;
    font-family: roboto;
    left: 570px;
    top: 200px;
    transform: scaleX(0.9); /* Initial transform */
    font-weight: 500;
    letter-spacing: 2px;
    animation: logAnimation 2s ease-in-out forwards; /* Apply animation */
}

/* Define keyframes for the animation */
@keyframes logAnimation {
    0% {
        transform: scaleX(0.9); /* Start state */
    }
    100% {
        transform: scaleX(1); /* End state */
    }
}




    .form{

        position: relative;
        left: 520px;
        top: 230px;
        padding: 20px;

    }
    .form1 , .form2{

        color: rgb(255, 255, 255);
        text-align: center;
        height: 20px;
        text-decoration: none;
        border: none;
        animation-name: form;
        animation-duration: 3s;
        animation-iteration-count: 1;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in-out;


    }

    .form1:focus{
        outline: none;
        border: none;
        box-shadow: none;
    }
 
    .form2:focus{
        outline: none;
        border: none;
        box-shadow: none;
    }


    @keyframes form{

        25% { background-color: rgb(149, 149, 149);
        
        }
        /* 50% { background-color: rgb(120, 120, 120); }
        75% { background-color: rgb(155, 155, 155); } */
        100% { background-color: rgb(191, 189, 189 , 0.3);
        height: 25px;
        
        } 
    }

    .div{
        display: inline-block;
        margin-bottom: 20px;
        color: red;
        border: none;
    }

    input{
        background-color:rgb(191, 189, 189 , 0.3) ;
    }
    
    .divlogin{
        display: inline-block;
        position: relative;
        margin: 40px;
        left: 15px;
    }

    .login{
        background-color: rgb(191, 189, 189 , 0.3);
        height: 29px;
        width: 60px;
        letter-spacing: 2px;
        border: none;
        color: white;
        position: fixed;
        cursor: pointer;
        animation-name: tr;
        animation-duration: 2s;
        animation-iteration-count: 1;
        animation-fill-mode: forwards;
        animation-timing-function: ease-in-out;
        font-family: Roboto;
    }

    .login:hover {
    animation-name: td;
    animation-duration: 1s;
    animation-timing-function: ease-in-out;
    animation-iteration-count: 1; /* Optional: to repeat the animation */
    color: white ;
    animation-fill-mode: forwards; /* Keep the final color after animation */
    font-weight: 700;

}   
@keyframes tr {
    25% { background-color: rgb(127, 84, 196); } /* Light pinkish color */
    50% { background-color: rgb(117, 45, 181); }   /* Your theme's deep blue-purple */
    75% { background-color: rgb(87, 22, 144);} /* Light blue for contrast */
    100% { background-color: rgb(56, 10, 96); } 
}
@keyframes td {
    25% { background-color: rgb(127, 84, 196); } /* Light pinkish color */
    50% { background-color: rgb(117, 45, 181); }   /* Your theme's deep blue-purple */
    75% { background-color: rgb(87, 22, 144);} /* Light blue for contrast */
    100% { background-color: rgb(56, 10, 96); }            /* Back to white */
    
}
 
.box {
    background-color: aliceblue;
    width: 200px;
    height: 250px;
    display: inline-block;
    position: absolute;
    top: 0;
    right: 0;
    animation: moveBubble 70s  infinite;
    opacity: 10%;
}

@keyframes moveBubble {
    0% {
        top: 0;
        right: 0;
        border-radius: 48% 52% 56% 44% / 43% 52% 48% 57% ;
    }
    50% {
        top: 50%;
        right: 50%;
        transform: translate(50%, -50%);
        border-radius: 69% 31% 56% 44% / 60% 82% 18% 40% ;
    }
    75% {
        top: 100%;
        right: 0;
        transform: translateY(-100%);
        border-radius: 88% 12% 82% 18% / 15% 37% 63% 85%  ;
    }
    100% {
        top: 0;
        right: 0;
        border-radius:48% 52% 56% 44% / 43% 52% 48% 57%  ;
    }
}
</style>
</head>

<body class="body">
    <div class="box"></div>
    <div class="box2"></div>
    <div class="log">
    
        Login

    </div>

    <form class="form">
        <div class="div">
            <input class="form1" type="email" placeholder="email" required  autofocus>
        </div>
        <div class="div2">
            <input class="form2" type="password" placeholder="password" required>

        </div>
        <div class="divlogin">
            <button class="login">Login</button>
        </div>
    </form>
   
</body>
</html>



