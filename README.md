# timer-function
var c=1
var m=0,h=0;
var timer=0;
function a()
    {
       timedCount();
     //   tracking()
        
    }
function timedCount()
 {

 c=c+1;
    if(c<60) {document.getElementById('timer').innerHTML=h+"h:"+m+"min:"+c+"s"}
    else if (c>60){ c=c%60;m=m+1;document.getElementById('timer').innerHTML=h+"h:"+m+"min:"+c+"s"};
     
    if(m<60){ document.getElementById('timer').innerHTML=h+"h:"+m+"min:"+c+"s"}
    else if(m>60){h=h+1;m=m%60}

 t=setTimeout("timedCount()",1000)
 }
    
function stopCount()
 {
 clearTimeout(t);
     time=c;
 }
