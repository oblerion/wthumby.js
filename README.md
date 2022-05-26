# wthumby.js
emulate [thumby](https://thumby.us/) on web with js api<br>
see API [here](https://github.com/oblerion/wthumby.js/wiki)
## example main.js

let dx=0;<br>
let dy=0;<br>
//-------new sprite(width,heigth,list)<br>
let spr1 = wtu.Sprite( 8, 8, [129, 66, 36, 24, 24, 36, 66, 129]);<br>
//-------main loop function<br>
WTU=function()<br>
{<br>
	&emsp;if(wtu.buttonU.Pressed()==true) dy=dy-1;<br>
	&emsp;if(wtu.buttonD.pressed()==true) dy=dy+1;<br>
	&emsp;if(wtu.buttonL.pressed()==true) dx=dx-1;<br>
	&emsp;if(wtu.buttonR.pressed()==true) dx=dx+1;<br>
  //---------------drawSprite(sprite,x,y)<br>
	&emsp;wtu.display.drawSprite(spr1,dx,dy);<br>
	&emsp;wtu.display.update();<br>
}
