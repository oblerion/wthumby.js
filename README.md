# wthumby.js
emulate [thumby](https://thumby.us/) on web with js api<br>
see API [here](https://github.com/oblerion/wthumby.js/wiki)
## example main.js
```js
let dx=0;
let dy=0;
//             sprite(width,heigth,list)
let spr1 = wtu.Sprite( 8, 8, [129, 66, 36, 24, 24, 36, 66, 129]);
//    main loop function
WTU=function()
{
	if(wtu.buttonU.Pressed()==true) dy=dy-1;
	if(wtu.buttonD.pressed()==true) dy=dy+1;
	if(wtu.buttonL.pressed()==true) dx=dx-1;
	if(wtu.buttonR.pressed()==true) dx=dx+1;
  //                      drawSprite(sprite,x,y)
	wtu.display.drawSprite(spr1,dx,dy);
	wtu.display.update();
}
```
