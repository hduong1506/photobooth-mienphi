```html
<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<title>Hello Kitty Photobooth</title>

<link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Quicksand:wght@500&display=swap" rel="stylesheet">

<style>

body{
margin:0;
font-family:Quicksand;
background:linear-gradient(#ffd6ec,#ffffff);
text-align:center;
}

/* title */

h1{
font-family:Pacifico;
color:#ff4da6;
font-size:50px;
}

/* camera */

video{
width:260px;
border-radius:20px;
box-shadow:0 0 20px pink;
}

/* strip */

#strip{

background:white;
width:280px;
margin:auto;
padding:10px;
border-radius:20px;
box-shadow:0 0 20px hotpink;

}

/* slot */

.slot{

width:260px;
height:180px;
background:#eee;
margin:10px auto;
border-radius:10px;
position:relative;
overflow:hidden;

}

.slot img{

width:100%;
height:100%;
object-fit:cover;

}

/* delete */

.delete{

position:absolute;
top:5px;
right:5px;
background:red;
color:white;
border:none;
border-radius:50%;
cursor:pointer;

}

/* upload */

.upload{

position:absolute;
bottom:5px;
left:5px;

}

/* button */

button{

background:linear-gradient(45deg,#ff4da6,#ff99cc);
border:none;
padding:10px 20px;
margin:5px;
color:white;
border-radius:20px;
cursor:pointer;

}

button:hover{

transform:scale(1.1);

}

/* frames */

#frames{

display:flex;
flex-wrap:wrap;
justify-content:center;

}

.frame{

width:70px;
height:140px;
margin:5px;
border:3px solid pink;
border-radius:10px;
cursor:pointer;

}

/* snow */

.snow{

position:fixed;
top:-10px;
color:white;
animation:fall linear infinite;

}

@keyframes fall{

to{

transform:translateY(110vh);

}

}

footer{

color:#ff4da6;
padding:20px;

}

</style>

</head>

<body>

<h1>Hello Kitty Photobooth</h1>

<video id="video" autoplay></video>

<br>

<button onclick="capture()">Chụp</button>

<button onclick="save()">Lưu ảnh</button>

<br><br>

<div id="strip"></div>

<h3>Chọn khung</h3>

<div id="frames"></div>

<footer>

được tạo bởi hduowgg

</footer>

<canvas id="canvas" style="display:none"></canvas>


<script>

/* snow */

for(let i=0;i<40;i++){

let snow=document.createElement("div")

snow.className="snow"

snow.innerHTML="❄"

snow.style.left=Math.random()*100+"%"

snow.style.animationDuration=5+Math.random()*5+"s"

snow.style.fontSize=10+Math.random()*20+"px"

document.body.appendChild(snow)

}


/* camera */

let video=document.getElementById("video")

navigator.mediaDevices.getUserMedia({video:true})

.then(stream=>video.srcObject=stream)



/* 4 slots fixed */

let strip=document.getElementById("strip")

let images=[null,null,null,null]


function render(){

strip.innerHTML=""

for(let i=0;i<4;i++){

let slot=document.createElement("div")

slot.className="slot"


if(images[i]){

let img=document.createElement("img")

img.src=images[i]

slot.appendChild(img)


let del=document.createElement("button")

del.innerHTML="x"

del.className="delete"

del.onclick=()=>{

images[i]=null

render()

}

slot.appendChild(del)

}


/* upload */

let upload=document.createElement("input")

upload.type="file"

upload.className="upload"

upload.onchange=e=>{

let file=e.target.files[0]

let reader=new FileReader()

reader.onload=()=>{

images[i]=reader.result

render()

}

reader.readAsDataURL(file)

}

slot.appendChild(upload)

strip.appendChild(slot)

}

}

render()


/* capture */

function capture(){

let canvas=document.getElementById("canvas")

canvas.width=260

canvas.height=180

let ctx=canvas.getContext("2d")

ctx.drawImage(video,0,0)


let index=images.findIndex(x=>x==null)

if(index!=-1){

images[index]=canvas.toDataURL()

render()

}

}


/* frames */

let frames=document.getElementById("frames")

let selectedFrame=null


for(let i=0;i<30;i++){

let c=document.createElement("canvas")

c.width=70

c.height=140

let ctx=c.getContext("2d")

ctx.strokeStyle=`hsl(${i*12},80%,70%)`

ctx.lineWidth=6

ctx.strokeRect(0,0,70,140)


c.className="frame"


c.onclick=()=>{

selectedFrame=c

alert("Đã chọn khung")

}


frames.appendChild(c)

}



/* save */

function save(){

let canvas=document.createElement("canvas")

canvas.width=280

canvas.height=800

let ctx=canvas.getContext("2d")


ctx.fillStyle="white"

ctx.fillRect(0,0,canvas.width,canvas.height)


images.forEach((src,i)=>{

if(src){

let img=new Image()

img.src=src

ctx.drawImage(img,10,10+i*190,260,180)

}

})


if(selectedFrame){

ctx.drawImage(selectedFrame,0,0,280,800)

}


let link=document.createElement("a")

link.download="photobooth.png"

link.href=canvas.toDataURL()

link.click()

}


</script>

</body>
</html>
```
