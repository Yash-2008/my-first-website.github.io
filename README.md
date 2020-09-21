<!doctype html>
<html>

<head>
   
   <title>My Frist Animation</title>
   
    <style>
        body {
            background-color: lightskyblue;
            overflow: hidden;
            animation-name: sky;
            animation-duration: 15s;
            animation-delay: 0s;
            animation-iteration-count: infinite;
            animation-fill-mode: both;
            animation-timing-function: linear;
        }

        #bush1{
            position: absolute;
            left: 0px;
            bottom: 400px;
            height: 30%;
        }
        
        #bush2{
            position: absolute;
            left: 500px;
            bottom: 400px;
            height: 30%;
        }
        
        #bush3{
            position: absolute;
            left: 1000px;
            bottom: 400px;
            height: 30%;
        }

        .road {
            position: absolute;
            left: 0px;
            bottom: 0px;
            height: 15%;
            width: 100%;
            background-color: darkslategray;

        }

        .divider {
            position: inherit;
            bottom: 50%;
            border-top: 10px dashed white;
            width: 100%;
        }

        .bus {
            position: inherit;
            bottom: 40%;
            width: 100%;
            animation-name: drive;
            animation-duration: 11s;
            animation-delay: 0s;
            animation-iteration-count: infinite;
            animation-fill-mode: both;
            animation-timing-function: linear;
        }

        .bus img {
            width: 10%;
        }

        .bike {
            position: inherit;
            bottom: 15%;
            width: 100%;
            animation-name: drive;
            animation-duration: 9s;
            animation-delay: 1s;
            animation-iteration-count: infinite;
            animation-fill-mode: both;
            animation-timing-function: linear;
        }

        .bike img {
            width: 5%;
        }

        #cloud1 {
            position: absolute;
            top: 10%;
            left: 10%;
            width: 17%;
        }

        #cloud2 {
            position: absolute;
            top: 15%;
            left: 45%;
            width: 9.4%;
        }

        #cloud3 {
            position: absolute;
            top: 10%;
            left: 70%;
            width: 15.9%;
        }

        .cloud img {
            width: 100%;
            opacity: 0.8;
        }

        .cloud {
            animation-name: cloud;
            animation-duration: 10s;
            animation-delay: 2s;
            animation-iteration-count: infinite;
            animation-fill-mode: both;
            animation-timing-function: linear;
        }

        /*Animation*/
        @keyframes drive {
            From {
                transform: translateX(-15%)
            }

            To {
                transform: translateX(100%)
            }
        }

        @keyframes cloud {
            0% {
                transform: translateX(5%)
            }

            25% {
                transform: translateX(30%)
            }

            50% {
                transform: translateX(50%)
            }

            75% {
                transform: translateX(30%)
            }

            100% {
                transform: translateX(5%)
            }
        }

        @keyframes sky {
            0% {
                background-color: lavender
            }

            50% {
                background-color: lightgoldenrodyellow
            }

            100% {
                background-color: lavender
            }
        }

    </style>
</head>

<body>
    <div id="bush1">
     <img src="mountain.png">
    </div>
    <div id="bush2">
     <img src="mountain.png">
    </div>
    <div id="bush3">
     <img src="mountain.png">
    </div>

    <div class="road">

        <div class="divider">
        </div>

        <div class="bus">
            <img src="bus.png">
        </div>

        <div class="bike">
            <img src="food-delivery.png">
        </div>

    </div>

    <div class="cloud" id="cloud1">
        <img src="cloud.png">
    </div>

    <div class="cloud" id="cloud2">
        <img src="cloud.png">
    </div>

    <div class="cloud" id="cloud3">
        <img src="cloud.png">
    </div>
</body>

</html>
