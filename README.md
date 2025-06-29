# HTML code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS-6"CSS Grid Layout"</title>
    <title>Loader Animation</title>
    <link rel="stylesheet" href="c:\users\goyal\Desktop\HTML\style02.css"/>
</head>
<body>
    <div class="container">
    <div id="Header">header(1row,12columns)</div>
   
    <div id="Navigation">navigation(1row,6columns)</div>
    <div id="Sidebar">sidebar(10row,3columns)</div>
    <div id="Main">main(9rows,6columns)</div>
    <div id="Ads">ads(10rows,3columns)</div>
    <div id="Footer">footer(1row,12columns)</div>
    </div>
    <br/><br/>
     <h1 style="text-align:center;">Loader</h1>
  <div class="loader"></div>
</body>
</html>

#CSS code

.container{
    
    height:100vh;
    
    margin:auto;
   grid-template-columns: repeat(12,1fr);
    grid-template-rows: repeat(12,1fr);
    grid-gap: 10px 10px;
    display:grid;
    font-size: 20px;
    padding:0;

}

#Header{
color:black;
border:4px solid whitesmoke;
border-top:0;
grid-column:1/span 12; 

}

#Navigation{
    grid-column:4/span 6;
}


#Sidebar{
    grid-column:1/span 3;
    grid-row:2/span 10;
    
}

#Main{
    grid-column:4/span 6;
    grid-row:3/span 9;
   
}

#Ads{
    grid-column:10/span 3;
    grid-row:2/span 10;
}

#Footer{
    grid-column: 1/span 12;
}

.container div{
    background-color: pink;
}


@media(min-width:720px){
    #Header{
color:black;
border:4px solid whitesmoke;
border-top:0;
grid-column:1/span 12; 

}

#Navigation{
    grid-column:1/span 12;
    grid-row:2;
}


#Sidebar{
    grid-column:1/span 3;
    grid-row:3/span 9;
    
}

#Main{
    grid-column:4/span 9;
    grid-row:3/span 9;
   
}

#Ads{
    grid-column:1/span 3;
    grid-row: 12;
   
}

#Footer{
    grid-column: 4/span 9 ;
    grid-row: 12;
}

.container div{
    background-color: pink;
    
}
}


body {
  margin: 0;
  padding: 0;
  font-family: sans-serif;
}

.grid-container {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  grid-template-rows: repeat(12, 1fr);
  gap: 10px;
  height: 100vh;
  padding: 10px;
}



.loader {
  border: 16px solid #f3f3f3;
  border-top: 16px solid goldenrod;
  border-radius: 50%;
  width: 120px;
  height: 120px;
  animation: spin 2s linear infinite;
  margin:auto;
}

@keyframes spin {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg); 
  }
}
















