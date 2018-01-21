<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
    <style>

      .dropdown-submenu {
        position: relative;
      }

      .dropdown-submenu .dropdown-menu {
        top: 0;
        left: 100%;
        margin-top: -1px;
      }
      a:link{
        text-decoration: none;
      }
      a:hover{
        text-decoration: none;
      }
      .ddtable{
        border-collapse: separate;
        border-spacing: 2px;
      }
      .ddtd{
        text-align: center;   
        font-size: 14px;
        background-color: #ffffff;
        height: 100px;
        width: 100px;
        border-radius: 10%;
        border: 1px solid #000000;
        font-style: sans-serif;
        font-weight: bold;
      }
      .ddimg{
        height: 100px;
        width: 100px;
        display: block;
        margin: auto;
        margin-top: 5px;
      }
      #grid{
        margin-left: 100px;
        height: 100px;
        width: 100px;
        background-color: crimson;
        display: inline-block;
        width: 110px;
        display: inline;
      }
      #bSTab{
      }
      .subtd{
        width: 110px;
        height: 110px;
        display: inline-block;
      }
      .yes{
        background-color: aqua;
      }
    </style>
    <script>
      var edit = true;
      //Drag and Drop
      function allowDrop(ev) {
        ev.preventDefault();
       /* console.log("dragging");*/
      }

      function drag(ev) {
        ev.dataTransfer.setData("text", ev.target.id);
      }
      
      function drop(ev) {
        ev.preventDefault();
        var data = ev.dataTransfer.getData("text");
        console.log(ev.target.className.slice(0, 3));
        var targetI = ev.target.id;
        console.log("targetI: " + targetI);
        var imgContainer = document.getElementById("container");
        
       /* while (imgContainer.firstChild){
        console.log("imgcontainer: " + imgContainer.firstChild);  imgContainer.removeChild(imgContainer.firstChild);
        }*/
                                    if(targetI == "container"){
          console.log("ran");
        ev.target.appendChild(document.getElementById(data));
        }
        else{
          console.log("Filed target id was: " + targetI);
        }
      }


    </script>
  </head>
  <body>
    <table id="grid" class="ddtable">
      <tr>
        <td id="container" class="yes ddtd" ondragover="allowDrop(event)" ondrop="drop(event)">

        </td> 
        <td id="container"  class="bob yes ddtd" ondragover="allowDrop(event)" ondrop="drop(event)">

        </td>
      </tr>
    </table>

    <p>test drag paragraph</p>
    <div class="dropdown" id="library">
      <button class="btn btn-default dropdown-toggle" type="button" data-toggle="dropdown">Selection Library
        <span class="caret"></span></button>
      <ul class="dropdown-menu">

        <table class="ddtable">
          <tr>
            <td class="ddtd">
              <li class="dropdown-submenu">
                <a class="test" href="#" tabindex="-1">
                  <img  src="https://docs.google.com/drawings/d/1qUrpfDUmIcf0zU7vjhHBJFlxIxIimIYSn1Vdm-S3Nrc/pub?w=617&h=634" class="ddimg"/> Bell Schedules
                </a>
                <!--Within Bell Dropdown-->
                <ul class="dropdown-menu">
                  <li><a tabindex="-1">
                    <table id="bSTab" class="ddtable">
                      <tr>
                        <td ondrop="drop(event)" ondragover="allowDrop(event)" class="subtd yes ddtd">
                          <img draggable="true" ondragstart="drag(event)" id="drag1" class="ddimg" src="https://docs.google.com/drawings/d/1feysTjEhlMzQQFhNqdhNcHAZ_n38CZkAxmfA-y-8_Zs/pub?w=585&h=564">
                        </td>
                        <td ondrop="drop(event)" ondragover="allowDrop(event)" class="subtd ddtd">
                          <img draggable="true" ondragstart="drag(event)" id="drag2" class="ddimg" src="https://docs.google.com/drawings/d/1IbmfpEzul9tlknRVSKhEib51S5TwcoyF4dlVAkWTvk8/pub?w=585&h=564">
                        </td>
                        <td ondrop="drop(event)" ondragover="allowDrop(event)" class="subtd ddtd">
                          <img draggable="true" ondragstart="drag(event)" id="drag3" class="ddimg"  src="https://docs.google.com/drawings/d/1bp-PFS9Vbc08gnBo--OYDvF9LZkZiaTmiKse1cEH1rY/pub?w=960&h=720">
                        </td>
                        
                      </tr>
                      <tr>
                        <td ondrop="drop(event)" ondragover="allowDrop(event)" class="subtd ddtd">
                          <img draggable="true" ondragstart="drag(event)" id="drag4" class="ddimg" src="https://docs.google.com/drawings/d/11fAucwi4nmZxvbFUpzo8n94NvoWf7pqjZQLdeg705R0/pub?w=612&h=562">
                        </td>
                      </tr>
                    </table></a>
                  </li>
                </ul>
              </li>

            </td>
            <td class="ddtd">
              <!--Club Drop Down-->
              <li class="dropdown-submenu">
                <a class="test" href="#" tabindex="-1">
                  <img  src="https://docs.google.com/drawings/d/1KG8IpF2xKzYg9IkuZ1ha7kOFgAA7BmuFhYV4Ro3v7aY/pub?w=789&h=661" class="ddimg"/> Clubs
                </a>
                <!--Within Club Dropdown-->
                <ul class="dropdown-menu">
                  <li><a tabindex="-1">
                    <table id="cTab" class="ddtable">
                      <tr>
                        <td ondrop="drop(event)" ondragover="allowDrop(event)" class="subtd ddtd">
                          <img draggable="true" ondragstart="drag(event)" id="draga" class="ddimg" src="https://docs.google.com/drawings/d/10vcoUQLCh7euJRoYDRq_xuSodOn17PCtNNHPsE1FSHA/pub?w=460&h=475">
                        </td>
                        <td ondrop="drop(event)" ondragover="allowDrop(event)" class="subtd ddtd">
                          <img draggable="true" ondragstart="drag(event)" id="dragb" class="ddimg" src="https://docs.google.com/drawings/d/1c7eAIK8fOWbWH5VnCivuslYzd-oh8PJjqc2QrvV5f3Y/pub?w=742&h=662">
                        </td>
                        <td ondrop="drop(event)" ondragover="allowDrop(event)" class="subtd ddtd">
                          <img draggable="true" ondragstart="drag(event)" id="dragc" class="ddimg" src="https://docs.google.com/drawings/d/109e0ic7-eGcdCBvqyWiD5iHhWtfFNBt1cgL0bTgSPoI/pub?w=839&h=710">
                        </td>
                      </tr>
                      <tr>
                        <td ondrop="drop(event)" ondragover="allowDrop(event)" class="subtd ddtd">
                          <img draggable="true" ondragstart="drag(event)" id="dragd" class="ddimg" src="https://docs.google.com/drawings/d/1S0Z2PePRZXgM39M4MPSZs2CZgEIzq4EgkSpGgM1F_OQ/pub?w=652&h=653">
                        </td>
                        <td ondrop="drop(event)" ondragover="allowDrop(event)" class="subtd ddtd">
                          <img draggable="true" ondragstart="drag(event)" id="drage" class="ddimg" src="https://docs.google.com/drawings/d/1hkzisEUEr_RLvOKgffj1fpAyzCH0OU-CC7ZBxhF45KE/pub?w=695&h=415">
                        </td>
                        <td ondrop="drop(event)" ondragover="allowDrop(event)" class="subtd ddtd">
                          <img draggable="true" ondragstart="drag(event)" id="dragf" class="ddimg" src="https://docs.google.com/drawings/d/1biPuMOF66t4V3xzWfDbXXigLN9O4dVPns56ePpDGByM/pub?w=818&h=717">
                        </td>
                      </tr>
                      <tr>
                        <td ondrop="drop(event)" ondragover="allowDrop(event)" class="subtd ddtd">
                          <img draggable="true" ondragstart="drag(event)" id="dragg" class="ddimg" src="https://docs.google.com/drawings/d/1RpphGR4s0eJ9F82qQcIw-ge1pVDmqkVP3SruUu_PdIw/pub?w=729&h=665">
                        </td>
                      </tr>
                    </table></a>
                  </li>
                </ul>
              </li>
            </td><td class="ddtd"></td>
          </tr>
          <tr><td class="ddtd"></td><td class="ddtd"></td><td class="ddtd"></td></tr>
          <tr><td class="ddtd"></td><td class="ddtd"></td><td class="ddtd"></td></tr>
        </table>

        <!-- <li class="dropdown-submenu">
<a class="test" tabindex="-1" href="#">New dropdown <span class="caret"></span></a>
<ul class="dropdown-menu">

<li><a tabindex="-1" href="#">2nd level dropdown</a></li>

<li class="dropdown-submenu">
<a class="test" href="#">Another dropdown <span class="caret"></span></a>
<ul class="dropdown-menu">
<li><a href="#">3rd level dropdown</a></li>
</ul>
</li>
</ul>
</li>

<li class="dropdown-submenu">
<a class="test" href="#" >hello</a>
<ul class="dropdown-menu">
<p>Bye</p>
</ul>
</li>-->
      </ul>

    </div>



    <script>
      $(document).ready(function(){
        $('.dropdown-submenu a.test').on("click", function(e){
          $(this).next('ul').toggle();
          e.stopPropagation();
          e.preventDefault();
        });
      });
    </script>

  </body>
</html>
