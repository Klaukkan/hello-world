# hello-world
Trying out GitHub
Trying out editing a branch version of README, as per tutorial. This seems like an easy way to manage coding new features to existing code.

Testiksi laitetaan tänne vaikka Frontend-kurssin JavaScript-harjoitus.

<script>
  function fibonacci() 
{ 
 var x = prompt("Anna haluamasi Fibonacchin luvun järjestysnumero", "0");
 
 var luku = parseInt(x); /*edellinen rivi antaa x:lle arvon Stringinä, täytyy muuttaa kokonaisluvuksi */
if (luku != null)
 {
	var tulos = 0;
   var montako = luku; //sijoitetaan luku montako-muuttujaan
   var i = 0; //laskuri
   var eka = 1;/*muuttujat edellisille luvuille*/
   var toka = 1;
   var fibona = 1; /*muuttuja fibonaccin luvulle*/
  
  	if (montako==1) /*erikoistapaukset 0,1 ja 2*/
  		 {
		return 1;
		} 		
		else if (montako==2) 
   		{
		return 1;
		}
		else if (montako==0) 
   		{
		return 0;
		} 		
  	else {
  		i = 3; //kertoo funktiolle että kyseessä ei ole 0, 1 tai 2
	  }
 	while (i<montako+1) {
	 
 		 /*lasketaan luku*/
 		 
	 	tulos = toka + eka;
	 	toka = eka;
	 	eka = tulos;
	 	i++;
	 }
 	document.getElementById('vastaus').innerHTML = "Fibonaccin luku järjestysnumerolla<b> "+luku+"</b> on "+tulos;
	return;
}
else{
fibonacci();
}
}
  </script>
