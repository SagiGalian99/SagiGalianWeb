# SagiGalianWebbody{
    margin: 0%;
    font-family: 'Courier New', Courier, monospace;
    background-image: url('bg.png');
}
button{
    cursor: pointer;
}
.navbar-container{
    display: inline-flex;
    width: 100%;
    height: 10%;
    background-color:rgb(20, 20, 20);
    align-items: center;
    justify-content: center;
}
.nav{
    font-family: 'Courier New', Courier, monospace;
    color: white;
    margin-left: 30px;
    width: 130px;
    height: 50px;
    background: none;
    outline: none;
    border: none;
    transition: 1s;
}
.nav-h1{
    font-family: 'Courier New', Courier, monospace;
    font-size: 30px;
    color: white;
    padding-right: 60px;
    background: none;
    outline: none;
    border: none;
    font-weight:lighter;
    transition: 1s;
}
.nav-h1:hover{
    padding-right: 100px;
    transition: 1s;
}
.nav:hover{
    background-color: antiquewhite;
    color: black;
    font-weight: bold;
    font-size: 20px;
    transition: 1s;
}
#description{
    display: none;
    text-align: center;
    width: 50%;
    height: 50%;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
}
#des-label{
    font-size: 30px;
}
#des-p{
    font-size: 20px;
    font-weight: bold;
}
#links{
    position: absolute;
    left:50%;
    transform: translate(-50%);
}
#blur{
    display:block;
    width: 100%;
    height: 100%;
    filter: blur(2px);
    transition: 1s;
}
#blur:hover{
    filter: blur(0px);
    transition: 1s;
}
#aboutme{
    width: 100%;
    height: 100%;
    display: none;
    text-align: center;
    justify-content: center;
}
#me{
    width: 160px;
    height: 160px;
    border-radius: 100px;
    transition: 2s;
}
#me:hover{
    width: 260px;
    height: 260px;
    border-radius: 200px;
    transition: 2s;
}
#for-p{
    position: absolute;
    top: 30%;
    left: 50%;
    transform: translate(-50%,-30%);
    width: 40%;
    height: 40%;
    font-size: 30px;
}
function perfectCircle(){
    document.getElementById("description").style.display = 'block';
    document.getElementById("links").style.display = 'none';
    document.getElementById("aboutme").style.display = 'none';
    const label = "Perfect Circle";
    const description = "Perfect circle is a website that check your drawing skills, you need to draw your best symmetrical circle around the mid point. you will get score by % on each paint"
    document.getElementById("des-label").innerHTML = label;
    document.getElementById("des-p").innerHTML = description;
}
function codeFaster(){
    document.getElementById("description").style.display = 'block';
    document.getElementById("links").style.display = 'none';
    document.getElementById("aboutme").style.display = 'none';
    const label = "Code Faster";
    const description = "Code faster is a website that will make you improve your coding typing skills, in this website you can choose between 3 diffrent coding languages. in every language you have the main keywords in the selected language. as long as you play with it you will get better and better. your coding life will be much easier"
    document.getElementById("des-label").innerHTML = label;
    document.getElementById("des-p").innerHTML = description;
}
function rollete(){
    document.getElementById("description").style.display = 'block';
    document.getElementById("links").style.display = 'none';
    document.getElementById("aboutme").style.display = 'none';
    const label = "Rollete";
    const description = "If you have to choose something or someone and you have no clue what to choose, this is the end of your problem, put the details and press the button, the luck will choose for you."
    document.getElementById("des-label").innerHTML = label;
    document.getElementById("des-p").innerHTML = description;
}
function normal(){
    document.getElementById("links").style.display = 'block';
    document.getElementById("description").style.display = 'none';
    document.getElementById("aboutme").style.display = 'none';
}
function aboutMe(){
    document.getElementById("links").style.display = 'none';
    document.getElementById("description").style.display = 'none';
    document.getElementById("aboutme").style.display = 'block';
}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>sagi</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="navbar-container">
        <button class="nav-h1" onclick="normal()">Links</button>
        <button class="nav" onclick="perfectCircle()">Perfect Circle</button>
        <button class="nav" onclick="codeFaster()">Code Faster</button>
        <button class="nav" onclick="rollete()">rollete</button>
        <button class="nav" onclick="aboutMe()">About Me</button>
    </div>
    <div id="description">
        <h1 id="des-label"></h1>
        <p id="des-p"></p>
    </div>
    <div id="links">
        <a href="https://sagigalian99.github.io/codeFaster/" target="_blank">
            <img src="codeFaster.png" alt="no availble" id="blur">
        </a>
        <a href=" https://sagigalian99.github.io/randomize/" target="_blank">
            <img src="rollete.png" alt="no availble" id="blur">
        </a>
        <a href="https://yosefmaman.github.io/perfectCircle.com.il/" target="_blank">
            <img src="perfectCircle2.png" alt="no availble" id="blur">
        </a>
    </div>
    <div id="aboutme">
        <div id="for-p">
            <img src="me.png" alt="no me" id="me">
            <p>So, my name is Sagi Galian and as you can see i love to code in my free time. I made this website so i can center all of my websites in one place and to show you some of my projects :)</p>
        </div>
    </div>

    <script src="code.js"></script>
</body>
</html>
