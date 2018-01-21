# Kiosk-Main
Starting the code from as far back as the static website
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Kiosk Main</title>
  </head>
  <style>
    *{
      background-color: #33097a;
      /*border: 1px dashed black;*/
      font-family: Sans-serif;
    }
    h1{
      margin:auto;
      text-shadow: -1px 0 black, 0 2px black, 1px 0 black, 0 -1px black;
      text-align: center;
      color: #f3f330;
      padding: 0px;}
    img{
      height: 100px;
      width: 100px;
      background-color: #ffffff;}
    td{
      //width: 150px;
      text-align: center;   
      font-size: 14px;
      /*}
      div{*/
      background-color: #ffffff;
      height: 130px;
      width: 100px;
      padding-left: 20px;
      padding-right: 20px;
      padding-top: 10px;
      border-radius: 10%;
      border: 2px solid #000000;
      opacity: .8675;
      font-style: sans-serif;
      font-weight: bold;}
    td:hover{
      opacity: 1;}
    a{
      text-decoration: none;
      background-color: #ffffff;
      color: #33097a;}
    div{
      background-color: #ffffff;}
    table{
      margin: auto;
      margin-top: -10px;
      border-spacing: 18px;
      margin-left: 200px;}
    #sug{
      margin: auto;
      margin-left: 554px;
      background-color: #FFFFFF;
      border-radius: 25%;
      border:2px solid #000000;
      text-align: center;
      color: #001A66;
      opacity: .8675;
      padding-left: 0;
      padding-right: 0;
      font-size: 20px;
      width: 120px;
      height: 60px;
      margin-top: -11px;
    }
    #sug:hover{
      opacity: 1;}
    #text{
      margin-top: 7px;
      font-size: 18px;
      border-radius: 25%;}
    h1{
      text-align: center;
      border-radius: 10%;}
    #day{
      width: 250px;
      background-color:#FFFFFF;
      float: right;
      border-radius: 5%;
      margin-top: 50px;
      height: 275px;
    }
    #innerday{
      height: 150px;
      width: 150px;
      background-color: #FFFFFF;
      margin: auto;
      margin-top: 15px;
      border: solid 3px #41474C;
      border-radius: 10%;}
    #innerday img{
      height:100px;
      width:100px;
      position: absolute;
      margin-left:25px;
      margin-top: 25px;
      background-color: #FFFFFF;}
    #day h1{
      margin:auto;
      margin-top: 10px;
      text-align: center;
      background-color: #FFFFFF;
    }
    p{
      background-color: #FFFFFF;
      text-align: center;
      font-size: 24px;}
    div img{
      height: 100px;
      width: 1200px;} 
    #Heading{
      margin-left: -115px;
      display:block;
    }
    #time{
      background-color: #33097a;
      margin-left: 1183px;
      font-size: 24px;
      display: none;}
  </style>
  <script>

    //Finds the number date
    var now = new Date();
    var start = new Date(now.getFullYear(), 0, 0);
    var diff = now - start;
    var oneDay = 1000 * 60 * 60 * 24;
    var num = Math.floor(diff / oneDay);
    //    document.write(num);

    var list = [
      "D", "B", "A", "B", "A","D", "D", "B", "A", "B", "A", "B", "E", "E", "E", "A", "B", "A", "B", "E", "E", "E", "E", "E", "E", "A", "D", "D", "B", "A", "B", "A", "B", 
    ]; 

    var day = num-1;
    var today = list[day];
  </script>
  <body>
    <h1 id="Heading"> Welcome to the Sayville Student Link Center</h1>
    <div id = "time">
      Hello
    </div>
    <div id="day">
      <h1 id="title"> Today is a(n):</h1>
      <div id="innerday"> 
        <img id="AA" src= 	"https://docs.google.com/drawings/d/12xMwZ02PMsJkiU56ft94bUanTbuRjPdvgWXN4EhEHpk/pub?w=476&h=476">
        <img id = "BB" src="https://docs.google.com/drawings/d/1mAD1ePBFZmerIeh7eWdYNUuqL_tyfb2iGkcVmWtg4B8/pub?w=581&h=617">
      </div>
      <h1 id="subDayText">Day</h1>
      <p id ="test"> 
      </p>
    </div>
    <script>
      var y = new Date();

     var m = new Date();
      var d = new Date();
      var q = m.getMonth();
      var x = q +1;
      var dd = d.getDate();
      document.getElementById("test").innerHTML = x + "/" + d.getDate() + "/" + y.getFullYear();
    </script>
    <table>
      <tr>
        <td>
          <a href="https://d157rqmxrxj6ey.cloudfront.net/ncameron/17088/"><img src= "https://docs.google.com/drawings/d/1qUrpfDUmIcf0zU7vjhHBJFlxIxIimIYSn1Vdm-S3Nrc/pub?w=617&h=634">BELL SCHEDULES
          </a>
        </td>

       <td>
          <a href="https://cl.castlelearning.com/review/clo/account/logon"><img src="https://docs.google.com/drawings/d/1RUgJz4ldHTbp-Mq0Vw0jdvEtTTr4Ge6eI-aAyNitGS8/pub?w=587&h=549">CASTLE LEARNING</a>

        </td>
        <td>
          <a href="https://classroom.google.com/h"><img src="http://yourcloudworks.co.uk/wp-content/uploads/2015/05/logo_classroom_64px_clr.png">CLASSROOM</a>
        </td>
        <td>
          <a href="https://d157rqmxrxj6ey.cloudfront.net/ncameron/17089/"><img src="https://docs.google.com/drawings/d/1KG8IpF2xKzYg9IkuZ1ha7kOFgAA7BmuFhYV4Ro3v7aY/pub?w=789&h=661">
            CLUBS</a>
        </td>
        
        <td>
          <a href="https://drive.google.com/drive/my-drive"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/ad/Logo_of_Google_Drive.svg/2000px-Logo_of_Google_Drive.svg.png">DRIVE</a>
        </td>
      </tr>
      <tr>
        <td>
          <a href="https://mail.google.com/mail/u/0/#inbox"><img src="http://screenshots.en.sftcdn.net/en/scrn/6654000/6654092/gmail-mobile-07-535x535.png">GMAIL</a>
        </td>
        <td>
          <a href="http://sayville.k12.ny.us/webpages/shslibrary/index.cfm"><img src="https://docs.google.com/drawings/d/1vZC9ZmroVAwMXY0Y9rrtXKtdpTxj-MYxeE47gW9KMx4/pub?w=551&h=612">HIGH SCHOOL LIBRARY</a>
        </td>
        <td> 
          <a href="https://www.noodletools.com/"><img src="https://docs.google.com/drawings/d/1u7CVLxjC8aGY43KcSi1fo_NietI3879l2CcCic5nsQ8/pub?w=731&h=564">NOODLE TOOLS</a>
        </td>
        <td><a href="https://sayville.esboces.org/campus/portal/sayville.jsp"><img src="https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcS2hsANn0TEEdkJ00WO0PlnX-0Jwjw7YJlHpN12272rLvKw75YJ">PARENT PORTAL</a>
        <td>  
          <a href="https://quizlet.com"><img src="https://docs.google.com/drawings/d/1edixGsvw5CJL1YrgPjoI-wB9UNeCwJCoqdDHLJXOn5Y/pub?w=484&amp;h=499"/>QUIZLET</a> 
        </td>
      </tr>
      <tr>
        <td>     
          <a href="http://sayville.k12.ny.us/files/44478/2016-17%20holiday%20calendar.pdf"><img src="https://docs.google.com/drawings/d/1Ch9O-ymgdp8hSgpZL6HPhNRJQ1wHCQTw3Rs37nnB5Nk/pub?w=789&h=552">SCHEDULED DAYS OFF</a>
        </td>
        <td>
          <a href="http://www.sectionxi.org/v2/schedules.asp?menu="><img src="https://docs.google.com/drawings/d/1eTgNEd83x0pTwpSg5mn34fo2PkccRuUJJMvbd0gIaDE/pub?w=572&h=650">SPORTS</a>
        </td>
        <td>
          <a href="https://thimbleprojects.org/ncameron/82638/"><img src="https://docs.google.com/drawings/d/1NwsFYBsUx3rHev5BIn6GmWfSNXJ7ytM0m9mijEuuZOY/pub?w=588&h=535">TEACHER WEBSITES</a>
        </td>
        <td>
          <a href="http://turnitin.com/"><img src="https://docs.google.com/drawings/d/1uHuqzxhJjgo6olrXEqoBHF2zavghLymHJFUuIpuw4-c/pub?w=786&h=700">TURNITIN</a>
        </td>
        <td>
          <a href="http://www.wordreference.com/"><img src="https://docs.google.com/drawings/d/18ZuT-Q5nsCzWgjAcsfW8ByhKRCHWJJIhGJJxgliEN1I/pub?w=321&h=276">WORD REFERENCE</a>
        </td>
      </tr>
    </table>
    <a href="https://docs.google.com/a/st.sayvilleschools.org/forms/d/1ghf3pjJQ32U7XWig5XfZNADCZWHgNhcFD9prmKPhLIA/viewform?usp=send_form"><div id="sug"><div id="text">Suggestions? Click Me!</div></div>
    </a>
    <script>
      if (today == 'A'){
        document.getElementById("BB").style.opacity = 0;
        document.getElementById("AA").style.opacity = 1;
        document.getElementById("title").innerHTML = "Today is an";
        document.getElementById("day").style.height = "335px";
      };
      if (today == 'B') {
        document.getElementById("BB").style.opacity = 1;
        document.getElementById("AA").style.opacity = 0;
        document.getElementById("title").innerHTML = "Today is a";
        document.getElementById("day").style.height = "335px";
      };
      if (today == 'E'){
        document.getElementById("BB").style.opacity = 0;
        document.getElementById("AA").style.opacity = 1;
        document.getElementById("title").innerHTML = "The next school day is an";
        document.getElementById("day").style.height = "375px";
      };
      if (today == 'D'){
        document.getElementById("BB").style.opacity = 1;
        document.getElementById("AA").style.opacity = 0;
        document.getElementById("title").innerHTML = "The next school day is a";
        document.getElementById("day").style.height = "375px";
      };
      if (today == 'S'){
        document.getElementById("BB").style.opacity = 0;
        document.getElementById("AA").style.opacity = 0;
        document.getElementById("title").innerHTML = "Have a nice Summer!";
        document.getElementById("day").style.height = "325px";
        document.getElementById("subDayText").innerHTML = "";
      };
      if (!(today == 'S' || today == 'A' || today == 'B' || today == 'D' || today == 'E')){
        document.getElementById("BB").style.opacity = 0;
        document.getElementById("AA").style.opacity = 0;
        document.getElementById("title").innerHTML = "Error 404:";
        document.getElementById("day").style.height = "325px";
        document.getElementById("subDayText").innerHTML = "Day Not Found";
      }; 

      //Finds the time
      var t = new Date();
      var tt = t.getMinutes();
      var h = new Date();
      var hh = h.getHours();
      var hhh = hh - 12
      if (tt < 10){
        document.getElementById("time").innerHTML = hhh + ":0" + tt;}
      else{
        document.getElementById("time").innerHTML = hhh + ":" + tt;}
        
    </script>
  </body>
</html>
