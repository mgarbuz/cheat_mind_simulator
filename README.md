<!DOCTYPE html>
<html>
<head>
    <meta http-equiv="content-type" content="text/html; charset=UTF-8">
    <title></title>
    <style type='text/css'>
            #test{
			width: 100px;
			height:100px;
                display:none;
            }
            #circle_red {
      width: 150px;
      height: 150px;
      -webkit-border-radius: 25px;
      -moz-border-radius: 25px;
      border-radius: 125px;
      background: red;
	  border: 1px solid #000
    }
    
    #circle_red_right {
      width: 150px;
      height: 150px;
      -webkit-border-radius: 25px;
      -moz-border-radius: 25px;
      border-radius: 125px;
      background: red;
	  border: 5px solid #090
    }
      #circle_yellow {
      width: 150px;
      height: 150px;
      -webkit-border-radius: 25px;
      -moz-border-radius: 25px;
      border-radius: 125px;
      background: yellow;
	  border: 1px solid #000
    }
    #circle_yellow_right {
      width: 150px;
      height: 150px;
      -webkit-border-radius: 25px;
      -moz-border-radius: 25px;
      border-radius: 125px;
      background: yellow;
	  border: 5px solid #090
    }
      #circle_green {
      width: 150px;
      height: 150px;
      -webkit-border-radius: 25px;
      -moz-border-radius: 25px;
      border-radius: 125px;
      background: green;
	  border: 1px solid #000
    }
    #circle_green_right {
      width: 150px;
      height: 150px;
      -webkit-border-radius: 25px;
      -moz-border-radius: 25px;
      border-radius: 125px;
      background: green;
	  border: 5px solid #090
    }
      #circle_grey {
      width: 150px;
      height: 150px;
      -webkit-border-radius: 25px;
      -moz-border-radius: 25px;
      border-radius: 125px;
      background: white;
	  border: 1px solid #000
    }
	
	
	
	.container{
    display: flex;
    flex-direction: row;
    justify-content: center;
    border: 0px solid black;
    padding: 20px;
}
#con1{
    width: 150px;
    border: 0px solid black;
    background-color: none;
    height: 150px;
    border-right: 0px;
}
#con2{
    width: 350px;
    border: 0px solid black;
    background-color: none;
    height: 300px;
}
#con3{
    width: 150px;
    border: 0px solid black;
    border-left: 0px;
    background-color: none;
    height: 150px;
}



#con21{
    width: 150px;
    border: 0px solid black;
    background-color: none;
    height: 150px;
    border-right: 0px;
}
#con22{
    width: 150px;
    border: 0px solid black;
    background-color: none;
    height: 150px;
}
#con23{
    width: 150px;
    border: 0px solid black;
    border-left: 0px;
    background-color: none;
    height: 150px;
}
#con24{
    width: 150px;
    border: 0px solid black;
    border-left: 0px;
    background-color: none;
    height: 150px;
}
#con25{
    width: 150px;
    border: 0px solid black;
    border-left: 0px;
    background-color: none;
    height: 150px;
}


#myCanvas
{
    display: block;
    margin: 0 auto;
}

    </style>

</head>
<body>
<center>
<font size='6'>
<h1>
<time>00:00:00</time>
</h1></font>

<div id="phase3" style="display:none"><font size='5'>Введите ответ. Кружочки меняют цвет при нажатии.</font></div>
<div id="main_panel"></div>
<div id="phase1" style="display:none"><font size='5'>Запомните первые 15 цветов.</font></div>
<div id="phase0" style="display:block">
<font size='5'>Задача - запомнить и воспроизвести в правильном порядке последовательность из 20 кружков красного, жёлтого и зелёного цветов.
 На первом этапе появляются 15 кружочков по три, на втором - 5 кружков. Результат считывается до первой ошибки. Удачи!
 
 
 </font></div>

<div id="second_panel">

<button id="strt" style="height:100px;width:200px;margin-top: 5%;"><font size='7'>СТАРТ</font></button>


<button id="chk" style="display:none;height:100px;width:150px"><font size='7'>ВВОД</font></button>
</div>

<button id="finish" style="display:none;height:100px;width:250px"><font size='7'>ФИНИШ</font></button>
<div id="result"></div>

<canvas id="myCanvas" width="700" height="200">
    Ваш браузер не поддерживает Canvas
</canvas>

<div class="container">
    <div id="con1"><button id="agn" style="display:none;height:100px;width:250px"><font size='7'>ПОВТОР</font></button></div>
    <div id="con2"></div>
    <div id="con3"><button id="nxt" style="display:none;height:100px;width:250px"><font size='7'>ДАЛЕЕ</font></button></div>
</div>


  <div id="follow" style="display:none;"><font size='5'> Присоединяйтесь!</font></div>
  <div id="references" class="container">
    <div id="con21" style="display:none;"><p><a href="https://vk.com/m_garbuz"><img src="vk.png" width="100" 
   height="100" alt="Пример"></a></p></div>
    <div id="con22" style="display:none;"><p><a href="https://t.me/math_garbuz"><img src="tg.png" width="100" 
   height="100" alt="Пример"></a></p></div>
    <div id="con23" style="display:none;"><p><a href="https://yappy.media/profile/620b0c1492294148a0b62e6727001a68?utm_source=url&utm_medium=share"><img src="yappi.png" width="100" 
   height="100" alt="Пример"></a></p></div>
   <div id="con24" style="display:none;"><p><a href="https://vk.com/razgon_praktika"><img src="razgon.png" width="100" 
   height="100" alt="Пример"></a></p></div>
   <div id="con25" style="display:none;"><p><a href="instagram.com/mish_garbuz"><img src="inst.png" width="100" 
   height="100" alt="Пример"></a></p></div>
</div>

<script type='text/javascript'>

            const color= ['red','yellow','green'];
            var image = document.getElementById("myCanvas");
            var randoms = Array.from({length: 20}, () => Math.floor(Math.random() * 3));	
			for (var j = 0; j < 17; j+=3) {//проверка того, что нет трёх одинаковых цветов подряд в первой фазе
				if((randoms[j]==randoms[j+1]) && (randoms[j+1]==randoms[j+2])){
					randoms[j]=0;
					randoms[j+1]=2;
					randoms[j+2]=1;
					}
				}

			for (var j = 0; j < 12; j+=3) {//проверка того, что нет двух подряд одинаковых троек. НЕ РАБОТАЕТ
				if((randoms[j]==randoms[j+3]) && (randoms[j+1]==randoms[j+4])&& (randoms[j+2]==randoms[j+5])){
					randoms[j]=0;
					randoms[j+1]=2;
					randoms[j+1]=1;
					randoms[j+3]=1;
					randoms[j+4]=2;
					randoms[j+5]=0;
					}
				}	
			for (var j = 15; j < 18; j++) {//проверка того, что в последних пяти кружках нет трёх подряд одинаковых цветов
				if((randoms[j]==randoms[j+1]) && (randoms[j+1]==randoms[j+2])){
					randoms[j]=1;
					randoms[j+1]=0;
					randoms[j+2]=2;
					}
				}				
            var p = 0;

            var i = 0, s = ["block","none"], t = [100,100]; //2 сек есть картинка, 1 сек нет
            var count = 0;
            var canvas = document.getElementById("myCanvas"), 
            context = canvas.getContext('2d');
            
            function switchColor(number) {
               var str_res = "";
               var color = document.getElementById('data_' + number).innerHTML;
               color++;
               color = color%3
               var r = color;
               if(r == 0) str_res += "<div id=\"circle_red\"></div>";
               if(r == 1) str_res += "<div id=\"circle_yellow\"></div>";
               if(r == 2) str_res += "<div id=\"circle_green\"></div>";
               document.getElementById("data_" + number).innerHTML = color;
               document.getElementById("circle_" + number).innerHTML = str_res;
        }
            function checkResult(min, sec, milisec) {
               var score = 0;
               for (let i = 0; i < randoms.length; i++) {
                   var answer = document.getElementById("data_"+i).innerHTML;
                   if (answer != randoms[i]) {
                      break;
                   }
                   if (answer == 0) document.getElementById("circle_"+i).innerHTML = "<div id=\"circle_red_right\"></div>"; 
                   if (answer == 1) document.getElementById("circle_"+i).innerHTML = "<div id=\"circle_yellow_right\"></div>";
                   if (answer == 2) document.getElementById("circle_"+i).innerHTML = "<div id=\"circle_green_right\"></div>";
                   score++;
               }
               document.getElementById("result").innerHTML = drawTableByArray(randoms, 4, 5);
               alert('Ваш результат: ' + score + '\nВаше время: ' + (min > 9 ? min : "0" + min) + ':' + sec + ':' + milisec + '\n\n P.S.: Подписывайтесь на мои соцсети! Ссылки внизу:) ');
            }

            function drawTableByArray(array, rows, columns) {
               var result = "<font size='7'>Правильный ответ:</font> \n\n\n <table>";
               for (let i = 0; i < rows; i++) {
                   result += "<tr>";
                   for (let j = 0; j < columns; j++) {
                       result += "<th>";
                       var r = array[i*columns + j];
	               if(r == 0) result += "<div id=\"circle_red\"></div>";
               	if(r == 1) result += "<div id=\"circle_yellow\"></div>";
               	if(r == 2) result += "<div id=\"circle_green\"></div>";
                       result += "</th>";
                   }
               }
               result += "</table>";
               return result;
            }


            window.onload = function(){

            var h1 = document.getElementsByTagName('h1')[0];
            var start = document.getElementById('strt');
            var next = document.getElementById('nxt');
            var check = document.getElementById('chk');
            var again = document.getElementById('agn');
            var milisec = 0;
            var sec = 0;
            var min = 0;
            var time;
            
            function clearTime() {
                   milisec = 0; sec = 0; min = 0;
            }

            function tick(){
		    milisec+=10;
		    if (milisec >= 100) {
			    milisec = 0;
			    sec++;
			    if (sec >= 60) {
				    sec = 0;
				    min++;
			    }
		    }
            }

            function add() {
		    tick();
		    h1.textContent = (min > 9 ? min : "0" + min) 
		    + ":" + (sec > 9 ? sec : "0" + sec)
		    + ":" + (milisec > 9 ? milisec : "0" + milisec);
		    timer();
            }

            function timer() {
            	time = setTimeout(add, 100);
            }

            //timer();
            //show();
			start.onclick = function() {
			clearInterval();
			document.getElementById("strt").style.display = "none";
			document.getElementById("phase0").style.display = "none";
			document.getElementById("phase1").style.display = "block";
			//document.getElementById("main_panel").innerHTML = "<button id='chk'>check</button>";
		    timer();
		    show();
            }

            check.onclick = function() {
            	//clearTimeout(time);
			   image.style.display = "none";
			   document.getElementById("phase3").style.display = "block";
               document.getElementById("main_panel").innerHTML=generateTable();
               document.getElementById("second_panel").style.display = "none";
               document.getElementById("finish").style.display = "block";
            }

            next.onclick = function() {
			image.style.display = "none";
			document.getElementById("nxt").style.display = "none";
			document.getElementById("agn").style.display = "none";
			p=15;
			phase2();
            }
            again.onclick = function() {
			document.getElementById("phase1").style.display = "block";
			document.getElementById("nxt").style.display = "none";
			document.getElementById("agn").style.display = "none";
		    p=0;
		    count=0;
		    i=0;
		    show();
            }
			
			finish.onclick = function() {
			clearTimeout(time);
			checkResult(min, sec, milisec);
			document.getElementById("finish").style.display = "none";
                       for (let i = 0; i < 20; i++) {
                           document.getElementById(i).onclick = "";
                       }
			document.getElementById("follow").style.display = "block";
			document.getElementById("con21").style.display = "block";	
			document.getElementById("con22").style.display = "block";
			document.getElementById("con23").style.display = "block";
			document.getElementById("con24").style.display = "block";
			document.getElementById("con25").style.display = "block";
            }



            function drawCircle(i, j, k, l , color) {
                   context.beginPath();
		    context.arc(i, j, k, l, Math.PI*2, false);
		    context.closePath();
		    context.stroke();
		    context.fillStyle = color;
		    context.fill();
            }
            
            function show() {
                   if (p >= 15) {
                      document.getElementById("agn").style.display = "block";
					  document.getElementById("nxt").style.display = "block";
					  document.getElementById("phase1").style.display = "none";
                      return;
                   }                   
                   drawCircle(210, 90, 50, 0, color[randoms[p]]);
                   drawCircle(350, 90, 50, 0, color[randoms[p+1]]);
                   drawCircle(500, 90, 50, 0, color[randoms[p+2]]);
                   image.style.display = "block";
                   p += 3;
                   setTimeout(hide, 2000);
            }

            function hide() {
                   image.style.display = "none";
                   setTimeout(show, 1000);
            }
            

	     function phase2() {
                   setTimeout(phase3, 1000);
	     }
             
             function phase3() {
                   context.clearRect(0, 0, 700, 200);
                   drawCircle(60, 90, 50, 0, color[randoms[p]]);
                   drawCircle(200, 90, 50, 0, color[randoms[p+1]]);
                   drawCircle(350, 90, 50, 0, color[randoms[p+2]]);
                   drawCircle(500, 90, 50, 0, color[randoms[p+3]]);
                   drawCircle(650, 90, 50, 0, color[randoms[p+4]]);
                   image.style.display = "block";
				   document.getElementById("chk").style.display = "block";
             }

            //show()

            function generateTable() {
               var result = "<table>" 
                            + generateRow(0)
                            + generateRow(5)
                            + generateRow(10)
                            + generateRow(15)
                            + "</table>";
               return result;
        }
        function generateRow(row) {
               var result = "<tr>" 
                          + generateCell(row+0) + generateCell(row+1) + generateCell(row+2) + generateCell(row+3) + generateCell(row+4)
			   + "</tr>";
               return result;
        }
        function generateCell(id) {
               var result = "<th id=\""+id + "\" onclick=\"switchColor('" + id + "')\">\
                   <div id=\"data_" + id + "\" style=\"display:none\">" + -1 + "</div>\
                   <div id=\"circle_" + id + "\">\
                        <div id=\"circle_grey\"></div>\
                   </div>\
               </th>";
               return result;
        }

            }					

</script>

</center>
</body>
</html>
