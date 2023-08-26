#   Universidad Mariano Galvez de Guatemala
    Ingenieria en Sistemas
    Curso: Algoritmos

Escriba un algoritmo para conversión de unidades de longitud, el programa debe recibir un número que es representado en centímetros. Luego preguntar a qué unidad se quiere convertir, las opciones son: metros, yardas, varas, pulgadas y pies.
Ejemplo:

El usuario ingresa 109 centímetros, luego elige la opción pies. El sistema deberá mostrar: 3.5761 pies. Debe escribirlo en Pseudocódigo, C++ y Python.

----

# Codigo en Pseint
    Algoritmo Conversion_Unidades
	//Declaracion de variables
	a<-0
	menu<-0
	Escribir "Ingrese su cantidad en Centimetros: ";
		leer a;
	Mientras a<=0 Hacer
		Escribir "Este numero no es valido, Introduzca otro";
		leer a;
		finmientras 
	Escribir "Seleccione la medida de conversion  en la que desea convertir sus centimetros: ";
	Escribir " ";
	Escribir "(1) Metros";
	Escribir "(2) Yardas";
	Escribir "(3) Varas";
	Escribir "(4) Pulgadas";
	Escribir "(5) Pies";
	Escribir " ";
		leer menu;
	escribir " ";
	//Opciones
	segun menu Hacer
		
		1: Escribir "La conversion deseada de centrimetros a Metros es";
			Escribir "Metros: ",a*0.01;
		2: escribir "La conversion deseada de centrimetros a Yardas es";
			Escribir "Yardas: ",a*0.0109361; 
		3: Escribir "La conversion deseada de centrimetros a Varas es";
			Escribir "Varas: ",a*0.01191;
		4: Escribir "La conversion deseada de centrimetros a Pulgadas es";
			Escribir "Pulgadas: ",a*0.393701;
		5: Escribir "La conversion deseada de centrimetros a Pies es";
			Escribir "Pies: ",a*0.0328084;
			
		De Otro Modo:
			Escribir "Usted ha ingresado una opcion incorrecta";
    	FinSegun
    FinAlgoritmo


## Ejecución en Pseint
- [Visualización del Usuario y del Programador](https://drive.google.com/file/d/1JC-H5-dwKVY6E0yiFgc-5GhxXzOVLfpw/view?usp=sharing)
-[Diagrama de flujo](https://drive.google.com/file/d/17PnCNhMasLQEJ7VDKe1_S64CWg5tNXt0/view?usp=sharing)

---

#   Codigo en C++
        #include <iostream>
        using namespace std;
        int main (){
            // Declaracion de variables
        float n, m, y, v, pu, pi;
        int opcion;
        cout<<"Ingrese su cantidad en Centimetros: ";
        cin>> n;
            // Menu
        cout<<"Seleccione la medida de conversion  en la que desea 
        convertir sus centimetros: "<<endl;
        cout<<"\n1. Metros \n2. Yardas \n3. Varas \n4. Pulgadas 
        \n5. Pies \n "<<endl;
        cin >>opcion;
            // opciones 
    switch(opcion)
    {
    case 1: 
		m= n*0.01;
		cout << "\nLa conversion deseada de centrimetros a Metros es:"<<m;
    		break;
    case 2:
		y= n*0.0109361;
		cout << "\nLa conversion deseada de centrimetros a Yardas es:"<<y;
		    break;
    case 3:
		v= n*0.01191;
		cout << "\nLa conversion deseada de centrimetros a Varas es:"<<v;
   		 break;
   	case 4:
		pu= n*0.393701;
		cout << "\nLa conversion deseada de centrimetros a pulgadas es:"<<pu;
   		 break;
   	case 5:
		pi= n*0.0328084;
		cout << "\nLa conversion deseada de centrimetros a pies es:"<<pi;
   		 break;
   		 
         // En dado caso el usuario ingrese un Numero que no
         se encuentra dentro del menu
    default: cout << "Usted ha ingresado una opcion incorrecta";
    }
    return 0;
    }
---
# Ejecución En C++
- [Visualización del Usuario y del Programador](https://drive.google.com/file/d/1MJ1EDOITggxzehfFOJNEzSFFR8IuyNQm/view?usp=drive_link)