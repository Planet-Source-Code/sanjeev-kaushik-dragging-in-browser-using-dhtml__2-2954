<div align="center">

## Dragging In Browser Using DHTML


</div>

### Description

Sharing the information with fellow programmers
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Sanjeev Kaushik](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/sanjeev-kaushik.md)
**Level**          |Advanced
**User Rating**    |3.5 (14 globes from 4 users)
**Compatibility**  |
**Category**       |[\.JS files](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/js-files__2-77.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/sanjeev-kaushik-dragging-in-browser-using-dhtml__2-2954/archive/master.zip)





### Source Code

```
<html>
<head>
 <title>Dragging In browser</title>
<meta name="Keywords" content="Dragging in DHTML by Sanjeev Kaushik" />
<meta name="Description" content="Dragging in DHTML by Sanjeev Kaushik,HTML,CSS,JavaScript,DHTML" />
<script language=javascript>
function go(){
if (event.button!=1)
		return;
	mydiv = eval("document.all.my");
	temp1 = mydiv.style.posLeft;
	temp2 = mydiv.style.posTop;
	xpos = event.clientX;
	ypos = event.clientY;
	xoff = temp1-xpos;
	yoff = temp2-ypos;
	mydiv.onmousemove = mymove;
}
function mymove(){
if (event.button==1){
  		x = event.clientX + xoff
		y = event.clientY + yoff;
		 mydiv.style.pixelLeft = x;
		mydiv.style.pixelTop =y
		return false;
	}
}
</script>
</head>
<body>
<div title="press left button and drag" align=center onmousedown="go()" id="my" style="position:absolute;left:100;top:100;width:150;background-color:maroon;filter:alpha(style=3);cursor:hand">
<font color=yellow>Sanjeev Kaushik</font>
<!-- you can also add any image here -->
</div>
</body>
</html>
```

