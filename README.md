<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>big-white</title>
    <style>
        *,body{
            margin: 0;
            padding: 0;
        }
        .wapper{
            position: relative;
            width: 500px;
            height: 700px;
        }
        .bg{
            position: absolute;
            width: 500px;
            height: 700px;
            background-color: #587070;
            overflow: hidden;
        }
        .boxone{
            width: 300px;
            height: 50px;
            margin: 0 auto;
            border: 4px solid #394946;
            border-top: none;
            box-shadow: 0 -1px 5px rgba(0,0,0,1); 
        }
        .boxtwo{
            width: 300px;
            height: 80px;
            margin: 0 auto;
            border: 4px solid #394936;
            box-shadow: 0 0 5px rgba(0,0,0,1), 0 0 10px rgba(0,0,0,.3) inset;
            background-color: #394946;
        }
        .boxthree{
            position: relative;
            width: 300px;
            height: 300px;
            margin: 0 auto;
            border: 4px solid #364936;
            box-shadow: 0 0 5px rgba(0,0,0,1), 0 0 10px rgba(0,0,0,.3) inset;
            background-color: #394946;
        }
        .boxthree:after {
            content: '';
            position: absolute;
            width: 95%;
            height: 97%;
            margin: 1%;
            border: 4px solid #364936;
            background-color: #2f3f4e;
        }
        .boxfour {
            width: 100%;
            height: 80px;
            margin: 2px auto;
            border-top: 4px solid #364936;
            border-bottom: 4px solid #364936;
            box-shadow: 0 0 5px rgba(0,0,0,.1), 0 0 10px rgba(0,0,0,.3) inset;
            background-color: #2c3733; 
        }
        .lineone{
            position: absolute;
            top: 625px;
            left: -41px;
            width: 165px;
            height: 3px;
            margin: 0 auto;
            transform: rotate(-240deg);
            background-color: rgba(0,0,0,.3);
        }
        .linetwo{
            position: absolute;
            top: 625px;
            right: -41px;
            width: 165px;
            height: 3px;
            margin: 0 auto;
            transform: rotate(240deg);
            background-color: rgba(0,0,0,.3);
        }
        .body{
            width: 480px;
            height: 700px;
            position: absolute;
        }
        .cpu{
            position: absolute;
            left: 270px;
            top: 170px;
            width: 30px;
            height: 30px;
            background-color: #e4e4e4;
            border-radius: 70% 100%;
            box-shadow: 0 2px 3px rgba(0,0,0,.2), 0 2px 3px rgba(255,255,255,1) inset;
            z-index: 2;

        }
        .heart {
            width: 16px;
            height: 20px;
            position: relative;
        }
        .heart:before {
            position: absolute;
            left: 10px;
            top: 10px;
            content:" ";
            width: 8px;
            height: 12px;
            border: 0 solid transparent; 
            border-radius: 25px 10px 0 0;
            background: #E24C4C;
            -webkit-transform: rotate(-45deg);
            -moz-transform: rotate(-45deg);
            -o-transform: rotate(-45deg);
            transform: rotate(-45deg);
        }
        .heart:after {
            position: absolute;
            left: 14px;
            top: 10px;
            content:" ";
            width: 8px;
            height: 12px;
            border: 0 solid transparent;
            border-radius: 10px 25px 0 0;
            background: #E24C4C;
            -webkit-transform: rotate(45deg);
            -moz-transform: rotate(45deg);
            -o-transform: rotate(45deg);
            transform: rotate(45deg);
        }
        .head {
            position: absolute;
            left: 177px;
            top: 67px;
            width: 110px;
            height: 76px;
            border-radius: 50% 45%;
            box-shadow: 0 10px 5px rgba(0,0,0,0.2);
            background: -webkit-linear-gradient(top, #fff 30%, #d6d6d6);
            z-index: 2;
        }
        .eyeleft {
            position: absolute;
            left: 20px;
            top: 30px;
            width: 12px;
            height: 12px;
            border-radius: 100%;
            background-color: #000;
            -webkit-animation: eye 2s ease infinite;
            -moz-animation: eye 2s ease infinite;
            -o-animation: eye 2s ease infinite;
            animation: eye 2s ease infinite;
        }
        .eyeright {
            position: absolute;
            left: 76px;
            top: 30px;
            width: 12px;
            height: 12px;
            border-radius: 100%;
            background-color: #000;
            -webkit-animation: eye 2s ease infinite;
            -moz-animation: eye 2s ease infinite;
            -o-animation: eye 2s ease infinite;
            animation: eye 2s ease infinite;
        }
        .eyeline{
            position: absolute;
            top: 36px;
            left: 30px;
            width: 50px;
            height: 1px;
            background-color: #000;
        }
        @keyframes eye{
            0%,20%, 100%{
                transform: scale(1,1);
            }
            10%{
                transform: scale(1,.2);
            }
        } 
        .trunk{
            position: absolute;
            left: 106px;
            top: 100px;
            z-index: 1;
        }
        .trunkone {
            position: absolute;
            left: 27px;
            top: 19px;
            width: 50px;
            height: 64px;
            border: 79px solid #eee;
            background: #eee;
            border-radius: 100%;
        }
        .trunktwo {
            position: absolute;
            left: 22px;
            top: 100px;
            width: 100px;
            height: 200px;
            background: #eee;
            -webkit-transform: rotate(12deg);
            -moz-transform: rotate(12deg);
            -o-transform: rotate(12deg);
            transform: rotate(12deg);
            box-shadow: -1px 1px 2px rgba(0,0,0,0.2);
        }
        .trunktwo:after {
            content: "";
            position: absolute;
            left: 113px;
            top: -27px;
            width: 100px;
            height: 200px;
            background: #eee;
            -webkit-transform: rotate(-24deg);
            -moz-transform: rotate(-24deg);
            -o-transform: rotate(-24deg);
            transform: rotate(-24deg);
            box-shadow: 1px 1px 2px rgba(0,0,0,0.2);
        }
        .trunkthree {
            position: absolute;
            left: 0px;
            top: 201px;
            width: 260px;
            height: 200px;
            border-radius: 100%;
            box-shadow: 0 10px 5px rgba(0,0,0,0.2);
            background: -webkit-linear-gradient(top, #eee 30%, #E4E4E4 60%, #e9e9e9 90%);
        }
        .handone {
            position: absolute;
            left: 16px;
            top: 196px;
            width: 320px;
            height: 143px;
            border-top: 76px solid #eee;
            border-radius: 32% 52%;
            -webkit-transform: rotate(-80deg);
            -moz-transform: rotate(-80deg);
            -o-transform: rotate(-80deg);
            transform: rotate(-80deg);
            z-index: 0;
        }
        .handtwo {
            position: absolute;
            left: 136px;
            top: 196px;
            width: 320px;
            height: 143px;
            border-top: 76px solid #eee;
            border-radius: 52% 32%;
            -webkit-transform: rotate(80deg);
            -moz-transform: rotate(80deg);
            -o-transform: rotate(80deg);
            transform: rotate(80deg);
            z-index: 0;
        }
        .fingerone {
            position: absolute;
            left: 88px;
            top: 427px;
            width: 20px;
            height: 48px;
            border-radius: 0 0 80% 50%;
            background: #eee;
            -webkit-transform: rotate(-32deg);
            -moz-transform: rotate(-32deg);
            -o-transform: rotate(-32deg);
            transform: rotate(-32deg);
        }
        .fingertwo {
            position: absolute;
            left: 104px;
            top: 426px;
            width: 20px;
            height: 43px;
            border-radius: 0 0 100% 45%;
            background: #eee;
            -webkit-transform: rotate(-32deg);
            -moz-transform: rotate(-32deg);
            -o-transform: rotate(-32deg);
            transform: rotate(-32deg);
        }
        .fingerthree {
            position: absolute;
            left: 364px;
            top: 427px;
            width: 20px;
            height: 48px;
            border-radius: 0 0 80% 50%;
            background: #eee;
            -webkit-transform: rotate(32deg);
            -moz-transform: rotate(32deg);
            -o-transform: rotate(32deg);
            transform: rotate(32deg);
        }
        .fingerfour {
            position: absolute;
            left: 353px;
            top: 426px;
            width: 20px;
            height: 43px;
            border-radius: 0 0 100% 45%;
            background: #eee;
            -webkit-transform: rotate(32deg);
            -moz-transform: rotate(32deg);
            -o-transform: rotate(32deg);
            transform: rotate(32deg);
        }
        .foot {
            position: absolute;
            left: 135px;
            top: 455px;
            z-index: 0;
        }
        .footone {
            position: absolute;
            left: 0;
            top: 0;
            width: 100px;
            height: 140px;
            background: -webkit-linear-gradient(left, #cdcdcd, #e3e3e3, #cdcdcd);
            border-radius: 10% 9% 22% 62%;
        }
        .foottwo {
            position: absolute;
            left: 100px;
            top: 0;
            width: 100px;
            height: 140px;
            background: -webkit-linear-gradient(left, #cdcdcd, #e3e3e3, #cdcdcd);
            border-radius: 10% 9% 62% 22%;
            box-shadow: -2px 0 2px rgba(0,0,0,0.1);
        }
    </style>
</head>
<body>
    <div class="wapper">
        <div class="bg">
            <div class="boxone"></div>
            <div class="boxtwo"></div>
            <div class="boxthree"></div>
            <div class="boxfour"></div>
            <div class="boxfive"></div>
            <div class="lineone"></div>
            <div class="linetwo"></div>
        </div>
        <div class="body">
            <div class="cpu">
                <div class="heart">
                    
                </div>
            </div>
            <div class="head">
                <div class="eyeleft"></div>
                <div class="eyeright"></div>
                <div class="eyeline"></div>
            </div>
            <div class="trunk">
                <div class="trunkone"></div>
                <div class="trunktwo"></div>
                <div class="trunkthree"></div>
            </div>
            <div class="hand">
                <div class="handone"></div>
                <div class="handtwo"></div>
                <div class="handthree"></div>
                <div class="handfour"></div>
                <div class="figureone"></div>
                <div class="figuretwo"></div>
                <div class="figurethree"></div>
                <div class="figurefour"></div>
            </div>
            <div class="foot">
                <div class="footone"></div>
                <div class="foottwo"></div>
            </div>
        </div>
    </div>
</body>
</html>
