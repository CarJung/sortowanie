<html>
<head>

<title>Strona</title>

 <link href="style.css" type="text/css" rel="stylesheet" />

</head>

<body>
  <div id="wrapper">
    <div id="logo">
    <a href="#">
        <h2><span class="light_logo">Rodzaje</span><br>sortowania</h2>
    <br>
    </a>
    </div>
    <div id="menu">
        <ul>
        <li><a href="README.md" class="active_tab">Strona główna</a></li>
        <li><a href="Podstrona 1.html">Sortowanie bąbelkowe</a></li>
        <li><a href="Podstrona 2.html">Sortowanie przez wybór</a></li>
        <li><a href="Podstrona 3.html">Sortowanie pozycyjne</a></li>
        <li><a href="Podstrona 4.html">Sortowanie kubełkowe</a></li>
        </ul>
    </div>
    <br><br><br><br><br><br>
    <div id="header">
    <img src="images/lol.jpg"/>
    <div id="title_head">
    <br><br><br>
	<hr width="1000" color="black">
    <h2>Witaj na naszej stronie internetowej</h2>
    <br>
    <div id="content">
    <div id="content_box">
    <h2>Kodeks w przestępczości internetowej</h2>
    <p>§ 1. Kto zabiera w celu przywłaszczenia cudzą rzecz ruchomą, podlega karze pozbawienia wolności od 3 miesięcy do lat 5.<br>  
     § 2. Tej samej karze podlega, kto bez zgody osoby uprawnionej uzyskuje cudzy program komputerowy w celu osiągnięcia korzyści majątkowej.     </p>
    <span id="content_box_rm"><a href="Odnośnikczytaj 1.html"> Czytaj dalej</a></span>
    </div>
    <div id="content_box" class="margin2">
    <h2>Artykuły prawne - najważniejsze</h2>
    <p>DDDDDDDDDDDDDDDDDDDD 
    </p>
    <span id="content_box_rm"><a href="Odnośnikczytaj 2.html"> Czytaj dalej</a></span>
    </div>
    </div>
    </div>
	<hr width="1000" color="black">
    <br>
    <div id="container">
    <h2>To może cię spotkać jeżeli nie będziesz ostrożny!!!</h2>
    <div id="box_photo">
    
    <img src="images/poli.png"  class="margin1" />
    <img src="images/kraty.png"  class="margin1" />
    <img src="images/Przechwytywanie.png"  class="margin1" />

   
    </div>
	<hr width="1000" color="black">
    <div id="content_box" class="margin1">
    <h2>Bibliografia</h2>
        <ul>
        <li><a href="https://www.google.pl/imghp?hl=pl&tab=wi">Google Grafika</a></li>
        <li><a href="http://podlaska.policja.gov.pl/pod/dzialania-policji/przestepczosc-gospodar/struktura-wydzialu/zespol-iii/piractwo-komputerowe/28415,Piractwo-komputerowe.html">Sortowanie bąbelkowe</a>
        <li><a href="#">Link 3</a></li>
        <li><a href="#">Link 4</a></li>
        </ul>
    </div>
    </div>
	<br>
	<hr width="1000" size="2" color="black">
    <big><big><marquee>Serdecznie zapraszamy! :D </marquee></big></big>
    <br>
    <hr width="1000" size="2" color="black">
    <br>
	<center>
<!-- START OF SCRIPT -->
<!-- For more scripts visit http://www.netpedia.com -->
<SCRIPT LANGUAGE="JavaScript">

<!-- Begin
monthnames = new Array(
"Styczeń",
"Luty",
"Marzec",
"Kwiecień",
"Maj",
"Czerwiec",
"Lipiec",
"Sierpień",
"Wrzesień",
"Październik",
"Listopad",
"Grudzień");
var linkcount=0;
function addlink(month, day, href) {
var entry = new Array(3);
entry[0] = month;
entry[1] = day;
entry[2] = href;
this[linkcount++] = entry;
}
Array.prototype.addlink = addlink;
linkdays = new Array();
monthdays = new Array(12);
monthdays[0]=31;
monthdays[1]=28;
monthdays[2]=31;
monthdays[3]=30;
monthdays[4]=31;
monthdays[5]=30;
monthdays[6]=31;
monthdays[7]=31;
monthdays[8]=30;
monthdays[9]=31;
monthdays[10]=30;
monthdays[11]=31;
todayDate=new Date();
thisday=todayDate.getDay();
thismonth=todayDate.getMonth();
thisdate=todayDate.getDate();
thisyear=todayDate.getYear();
thisyear = thisyear % 100;
thisyear = ((thisyear < 50) ? (2000 + thisyear) : (1900 + thisyear));
if (((thisyear % 4 == 0) 
&& !(thisyear % 100 == 0))
||(thisyear % 400 == 0)) monthdays[1]++;
startspaces=thisdate;
while (startspaces > 7) startspaces-=7;
startspaces = thisday - startspaces + 1;
if (startspaces < 0) startspaces+=7;
document.write("<table border=2 bgcolor=black ");
document.write("bordercolor=black><font color=#000000>");
document.write("<tr><td colspan=7><center><strong>" 
+ monthnames[thismonth] + " " + thisyear 
+ "</strong></center></font></td></tr>");
document.write("<tr>");
document.write("<td align=center>N</td>");
document.write("<td align=center>P</td>");
document.write("<td align=center>W</td>");
document.write("<td align=center>Ś</td>");
document.write("<td align=center>C</td>");
document.write("<td align=center>P</td>");
document.write("<td align=center>S</td>"); 
document.write("</tr>");
document.write("<tr>");
for (s=0;s<startspaces;s++) {
document.write("<td> </td>");
}
count=1;
while (count <= monthdays[thismonth]) {
for (b = startspaces;b<7;b++) {
linktrue=false;
document.write("<td>");
for (c=0;c<linkdays.length;c++) {
if (linkdays[c] != null) {
if ((linkdays[c][0]==thismonth + 1) && (linkdays[c][1]==count)) {
document.write("<a href=\"" + linkdays[c][2] + "\">");
linktrue=true;
      }
   }
}
if (count==thisdate) {
document.write("<font color='#FF0000'><strong>");
}
if (count <= monthdays[thismonth]) {
document.write(count);
}
else {
document.write(" ");
}
if (count==thisdate) {
document.write("</strong></font>");
}
if (linktrue)
document.write("</a>");
document.write("</td>");
count++;
}
document.write("</tr>");
document.write("<tr>");
startspaces=0;
}
document.write("</table></p>");
// End -->
</SCRIPT>
</center>
    <div id="footer">
    <p>©Copyright Michał Durman i Krzysztof Wróbel
    </div>
    </div>
</body>
</html>
