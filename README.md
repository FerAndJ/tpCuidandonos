# tpCuidandonos

Integrantes:
  Fernando Juncos, 
  Alexia Deza

Punto 2: Pseudo código de calculo de tiempo

int calcularTiempo([Parada]){
	
int tiempoTotal = 0

for(i=0. i< [Parada].lenght, i++){
 
 tiempoTotal = tiempoTotal + parada[i].tiempoRecorrido(parada[i-1].getDireccion()) + parada[i].getMinutosEspera()

}



return tiempoTotal
}



int calcularTiempoEntreParadas(parada, paradaAnterior) {
	
	int tiempo = parada.tiempoRecorrido(paradaAnterior.getDireccion()) + parada.getMinutosEspera()

	return tiempo;

}

Patrones de diseño utilizados:

Utilizamos un patron Adapter, por medio de la clase Adapter Distancias, para lograr una mayor modularidad y cohesion, al tener una clase aparte que se encargue de esos calculos
y delegar esta responsabilidad fuera de las interfaces de usuarios, de esta forma, si se quiere cambiar la logica para este calculo de distanicas, solo necesitariamos referencias
a otra clase adapter.



  

  
