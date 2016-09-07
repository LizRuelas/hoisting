+++ Codigo Inicial
var feature = "closures"; 

(function () {     
	if ( typeof feature === "undefined" ){         
		var feature = "callbacks";         
		console.log("JS coders love its " + feature );     
	} else {         
		console.log("JS developers love its " + feature );     
	} 
})();

+++ Codigo Modificado
var feature = "closures"; 

(function () {     
	if ( typeof feature === "undefined" ){         
		feature = "callbacks";         
		console.log("JS coders love its " + feature );     
	} else {         
		console.log("JS developers love its " + feature );     
	} 
})();

+++ ARGUMENTO
El var declarado en la linea 6 hace que el interprete "Eleve" mi variable asi :
(function () {  
	 var feature; // ----> la variable esta elevada
	if ( typeof feature === "undefined" ){         
		feature = "callbacks";         
		console.log("JS coders love its " + feature );//----> undefined     
	} else {         
		console.log("JS developers love its " + feature );     
	} 
})();

al eliminar el var de la linea 6 ya el interprete ya no "Eleva" la variable 
es decir ya no es undefined asi imprimira el ELSE.

