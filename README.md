<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Merriweather:ital,wght@0,300;0,400;0,700;0,900;1,300;1,400;1,700;1,900&family=Playwrite+MX:wght@100..400&display=swap" rel="stylesheet">
<div id="wall">
    <div id="circleBlur"></div>
        <div id="baseCircle">
            <div id="bigCircle"></div>
            <div id="bigCircle2"></div>
            <div id="bigCircle3"></div>
        </div>
    <span id="name">Hello</span>
</div>

<style>
*{
 font-family: "Merriweather", serif;
}
@keyframes move {
	100% {
		transform: rotate(360deg);
	}
}
#wall{
    display:flex;
    justify-content:center;

}
/* #circleBlur{
    width:400px;
    height:400px;
    position:absolute;
    z-index:1;
} */
#baseCircle{
z-index:0;
width:400px; 
height:400px; 
overflow: hidden;
transform: translate3d(0, 0, 0);
display:flex;
justify-content:center;

}
#bigCircle{
width:610px; 
height:610px; 
background-color:rgba(0,0,255,0.2);
border-radius:45%;
position:absolute;
top:-80%;
animation: move 3s infinite linear;
}
#bigCircle2{
width:600px; 
height:600px; 
background-color:rgba(100,100,255,0.2);
border-radius:45%;
position:absolute;
top:-80%;
animation: move 5s infinite linear;
}
#name{
    position:absolute;
    display:flex;
    align-items:center;
    height:300px;
    width:400px;
    justify-content:center;
    color:white;
    font-size:30px;
}

</style>
