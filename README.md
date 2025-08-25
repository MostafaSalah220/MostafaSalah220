
<html lang="en">
<head>
<meta charset="UTF-8">

<style>
*{margin:0;padding:0;box-sizing:border-box;}
#Hi{padding:2vw;font-size:10vw;font-family:cursive;align-items:center;color:#FFFFFF;font-weight:600;}
body{display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:100vh;background:#2d2d2d;}
.box{position:relative;background:#0f253d;height:200px;border-radius:10px;display:flex;justify-content:center;align-items:center;}
@property --deg{syntax:'<angle>';inherits:true;initial-value:0deg;}
.box::before,.box::after{content:"";position:absolute;top:0;left:0;height:100%;width:100%;background:conic-gradient(from var(--deg) at center,#00c3ff,#4d0199,#6300c6,#009dcd);border-radius:inherit;z-index:-2;padding:2px;animation:autoRotate 8s linear infinite;}
.box::after{filter:blur(10px);}
@keyframes autoRotate{to{--deg:360deg;}}
h2{position:relative;font-size:10vw;color:colorCycle;-webkit-text-stroke:0.2vw #383d52;text-transform:uppercase;}
h2::before{content:attr(data-text);position:absolute;top:0;left:0;width:0;height:90%;color:#BB86FC;-webkit-text-stroke:0vw #2D2D2D;border-right:2px solid #BB86FC;overflow:hidden;animation:animate 6s linear infinite,colorCycle 18s linear infinite;}
@keyframes colorCycle{0%{color:#BB86FC;}33%{color:#03DAC5;}66%{color:#FF0266;}100%{color:#BB86FC;}}
@keyframes glowPulse{0%,100%{text-shadow:0 0 5px currentColor,0 0 5px currentColor,0 0 6px currentColor;}50%{text-shadow:0 0 10px currentColor,0 0 10px currentColor,0 0 15px currentColor;}}
@keyframes animate{0%,10%,100%{width:0;}70%,90%{width:100%;}}
.Iam{padding:2em 2em;font:normal 4.5vw/5vw Montserrat,sans-serif;text-align:center;color:#999;}
.Iam p{height:80px;float:left;margin-right:0.3em;}
.Iam b{float:left;overflow:hidden;position:relative;height:5vw;top:0.1vw;}
.Iam .innerIam{display:inline-block;color:#e74c3c;position:relative;white-space:nowrap;top:0;left:0;-webkit-animation:move 5s;-moz-animation:move 5s;-ms-animation:move 5s;-o-animation:move 5s;animation:move 5s;-webkit-animation-iteration-count:infinite;-moz-animation-iteration-count:infinite;-ms-animation-iteration-count:infinite;-o-animation-iteration-count:infinite;animation-iteration-count:infinite;-webkit-animation-delay:2s;-moz-animation-delay:2s;-ms-animation-delay:2s;-o-animation-delay:2s;animation-delay:2s;}
@keyframes move{0%{top:0;}20%{top:-5vw;}40%{top:-10vw;}60%{top:-15vw;}80%{top:-20vw;}}
@-webkit-keyframes move{0%{top:0;}20%{top:-5vw;}40%{top:-10vw;}60%{top:-15vw;}80%{top:-20vw;}}
@-moz-keyframes move{0%{top:0;}20%{top:-5vw;}40%{top:-10vw;}60%{top:-15vw;}80%{top:-20vw;}}
@-o-keyframes move{0%{top:0;}20%{top:-5vw;}40%{top:-10vw;}60%{top:-15vw;}80%{top:-20vw;}}
@keyframes move{0%{top:0;}20%{top:-5vw;}40%{top:-10vw;}60%{top:-15vw;}80%{top:-20vw;}}
.terminal{font-family:monospace;color:#00FF00;background-color:black;padding:2em;border-radius:10px;width:60vw;height:30vw;display:flex;flex-direction:column;justify-content:start;gap:0.5em;font-size:2vw;line-height:1.8;}
.typing,.typing1,.typing2{border-right:2px solid #00FF00;white-space:nowrap;overflow:hidden;display:inline-block;}
.typing{width:0;animation:typing 2s steps(13,end) 0s forwards,blink 0.8s step-end 2s;}
.typing1{width:0;animation:typing1 2s steps(7,end) 2s forwards,blink 0.8s step-end 4s;}
.typing2{width:0;animation:typing2 3s steps(10,end) 4s forwards,blink 0.8s step-end infinite;}
@keyframes typing{from{width:0;}to{width:13ch;}}
@keyframes typing1{from{width:0;}to{width:7ch;}}
@keyframes typing2{from{width:0;}to{width:10ch;}}
@keyframes blink{0%,100%{border-color:transparent;}50%{border-color:#00FF00;}}
</style>
</head>
<body>
<div id="Hi">Hi There <br><spam style="align-items:left">I am</spam></div>
<div class="box"><h2 data-text="Mostafa.Salah">Mostafa.Salah</h2></div>
<div class="Iam"><p>I like</p><b><div class="innerIam">Problem solving<br />Web development<br />helping others<br />Electronics<br />make things easier</div></b></div>
<div class="terminal">
<p>> Skills</p>
<p><span class="typing">▍ HTML, CSS </span></p>
<p><spam class="typing1">▍ SQL</spam></p>
<p><spam class="typing2">▍ C++, C</spam></p>
</div>
</body>
</html>
