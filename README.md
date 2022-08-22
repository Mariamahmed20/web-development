# web-development
 web development/css grid/html/css  
 a simple css grid for beginners
 <!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title> grid </title>
  <style> 
.container{
  display: grid;
  width: 100%;
  margin: auto;
  grid-gap: 50px;
  border: 2px solid orange;
  justify-content: center;
  grid-template-columns: 100px 200px ;
  grid-template-rows: 300px;
  grid-template-areas: "hd hd hd hd hd hd hd hd"
      "sd sd sd main main main main main"
      "ft ft ft ft ft ft ft ft";


}
.box{
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  border: 1px solid red;
  padding: 15px;
}
#one{
  grid-area: hd;
}
#two{
  grid-area:main  ;
}
#three{
  grid-area: ft;
}
#four{
  grid-area: sd;
}

  </style>

</head>
<body>
<div class="container">
  <div class="box" id="one"> box 1</div>
  <div class="box" id="two">box 2 </div>
  <div class="box" id="three"> box 3</div>
  <div class="box" id="four"> box 4</div>
</div>
</body>
</html>
