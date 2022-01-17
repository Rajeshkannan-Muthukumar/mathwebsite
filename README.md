# Web Page for Mathematical Calculations

## AIM:

To design a static website with validation to perform mathematical calculations in client side.

## DESIGN STEPS:

### Step 1:

Requirement collection.

### Step 2:

Creating the layout using HTML and CSS.

### Step 3:

Write javascript to perform the calculations.

### Step 4:

Include regularexpression based input validation.

### Step 5:

Validate the layout in various browsers.

### Step 6:

Validate the HTML code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Volume</title>
    <style>
        * {
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
body {
  background-color:rgb(133, 125, 245);
}
.container {
  width: 1080px;
  margin-left: auto;
  margin-right: auto;
}
.content {
  display: block;
  width: 100%;
  background-color: #E6E6FA;
  min-height: 500px;
  margin-top: 150px;
}

h1{
    text-align: center;
    padding-top: 50px;
    color: rgb(133, 125, 245);
}
.formelement{
    text-align: center;
    font-size:xx-large;
    margin-top: 5px;
    margin-bottom: 5px;

}
    </style>
</head>
<body><div class="container">
  <div class="content">
            <h1>VOLUME OF  A CYLINDER</h1>
            <form>
                <div class=formelement>
                    <lable for="bedit">Radius:</lable>
                    <input type="text" id="bedit" value=""/>Meters
                </div><br>
                <div class=formelement>
                    <lable for="aedit">Height:</lable>
                    <input type="text" id="aedit" value=""/>Meters
                </div><br>
                
                <div class=formelement>
                    <input type="button" value="CALCULATE VOLUME" id="calbutton1"/>
                </div>
                <div class=formelement>
                    <lable for="cedit">Volume:</lable>
                    <input type="text" id="cedit" readonly="0"/>Cubic Meters
                </div><br>
               
            </form>
        </div>
        <script type="text/javascript">
            var button;
            button=document.querySelector("#calbutton1");
            button.addEventListener("click",function(){
                var atext,btext,ctext;
                var aval,bval,cval;
                atext=document.querySelector("#aedit");
                btext=document.querySelector("#bedit");
                ctext=document.querySelector("#cedit");

                aval=parseInt(atext.value);
                bval=parseInt(btext.value);
                cval=22/7*aval*bval*bval;
                ctext.value=cval;
                ctext.value=cval;
            });
        </script>
         <div class="container">
        <div class="content">
            <h1>AREA OF A RECTANGLE</h1>
            <form>
                <div class="formelement">
                  <lable for="lengthedit">LENGTH:</lable>
                  <input type="text" id="lengthedit" value=" "/>Meters
                </div><br>
                <div class="formelement">
                  <lable for="breadthedit">BREADTH:</lable>
                  <input type="text" id="breadthedit" value=" "/>Meters
                </div><br>
                <div class="formelement">
                  <input type="button" value="CALCULATE AREA" id="calbutton2"/>
                </div><br>
                <div class="formelement">
                  <lable for="areaedit">AREA:</lable>
                  <input type="text" id="areaedit" readonly="0"/>Square Meters
                </div><br>
                <div class="formelement">
               
                </div><br>
                
            </form>
    
            </div>
        </div>
        <script type="text/javascript">
          var button;
          button=document.querySelector("#calbutton2");
          button.addEventListener("click",function(){
            
              var lengthtext,breadthtext,areatext;
              var aval,bval,cval;
    
              lengthtext=document.querySelector("#lengthedit");
              breadthtext=document.querySelector("#breadthedit");
              areatext=document.querySelector("#areaedit");
      
              aval=parseInt(lengthtext.value);
              bval=parseInt(breadthtext.value);
              cval=aval*bval
              areatext.value=cval;
        
      
            });
      
        </script> 
        <script type="text/javascript">
  var button;
  button = document.querySelector("#calbutton1");
  button.addEventListener("click", function () {
    var atext, btext, ctext;
    var aval, bval, cval;
    atext = document.querySelector("#aedit");
    btext = document.querySelector("#bedit");
    ctext = document.querySelector("#cedit");

    if(Number(atext.value)&&Number(btext.value))
    {
      aval=parseInt(atext.value);
      bval=parseInt(btext.value);
    }
    else{
      window.alert("enter only number");
    }


    

    cval = 3.14 * aval * aval * bval;
    ctext.value = "" + cval;
  });
</script>
<script type="text/javascript">
  var button;
  button = document.querySelector("#calbutton2");
  button.addEventListener("click", function () {

   var lengthtext,breadthtext,areatext;
   var aval,bval,cval;
    lengthtext=document.querySelector("#lengthedit");
    breadthtext=document.querySelector("#breadthedit")
    areatext=document.querySelector("#areaedit");
      
    if(Number(lengthtext.value)&&Number(breadthtext.value))
    {
      aval=parseInt(lemgthtext.value);
      bval=parseInt(breadthtext.value);
    }
    else{
      window.alert("enter only number");
    }
    
    cval=aval*bval
    areatext.value=cval;
  });

</script>
</div>
  
</body>
</html>
```



## OUTPUT:
![OP](https://user-images.githubusercontent.com/93901857/149091878-b77dd6ce-768d-4f09-8fd0-3e19c6af65a4.jpg)
# ERROR
![ERROR 1](https://user-images.githubusercontent.com/93901857/149792114-4a549cab-c897-4296-82a8-a5bddbaa02f6.jpg)
![ERROR 2](https://user-images.githubusercontent.com/93901857/149792124-e2889d6e-aedd-4430-9da1-c9c6067d7539.jpg)

## Result:

Thus a website is designed to perform mathematical calculations in the client side.
