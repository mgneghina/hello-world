# hello-world
Just a sample repository
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Grumpy Cat</title>
      <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <img id="cat" class=""
         src="http://makeameme.org/media/templates/120/grumpy_cat.jpg" alt="" width="120" height="120">
  </body>
</html>

#cat {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 120px;
  height: 120px
  margin: -60px 0 0 -60px;
}
.image {
-webkit-animation:spin 4s linear infinite;
-moz-animation:spin 4s linear infinite;
animation: spin 4 s linear infinite;
}

@-moz-keyframes spin {100% { -moz-transform: rotate(360deg);}}
@-webkit-keyframes spin {100% { -webkit-transform: rotate(360deg); transform:rotate(360deg);}}

let image = document.querySelector("cat")
image.oneclick = toggleClass;
function toggleClass(){
  if(image.className == 'image'){
      image.className = ''
  } else {
      image.className = 'image'
  }
}
