<script type="text/javascript">

function getLocation(){
    var arr = document.domain.split('.');
    if(arr.length === 2){
        return document.domain;
    }
    if(arr.length > 2 && arr[0] !== 'www'){
      return arr.slice(1).join('.')
    } 
    return arr.slice(1).join('.') 
}

rootdomin=getLocation(window.location.host) ;

var fabulist = new Array(
	"990917.com",
	"990972.com",
	"990973.com",
	"990912.com",
	//"979165.com",
	"979172.com",
	"979315.com",
	"979276.com",
	"979283.com",
	"979253.com",
	//"979351.com",
	//"979176.com",
	"979327.com",
	"979236.com",
	//"979582.com",改56pe.com跳转使用
	//"979521.com",
	"979612.com",
	"979613.com",
	"979513.com",
	//"979920.com",
	) ;

var jump = fabulist.indexOf(rootdomin);  
var jumpurl = fabulist[Math.floor(Math.random()*fabulist.length)];

//document.write(jumpurl)

   if(jump<0){
        window.location.href = "http://www."+jumpurl;
    }
</script>
