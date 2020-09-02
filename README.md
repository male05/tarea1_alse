# tarea1_alse
#crear archivo 
#include<iostream>
#include<stdlib.h>
#include<fstream>
using namespace std;
  
  int main(){
   escribir();
   
   return 0;
  }
  
  void escribir(){
  string numeros;
  ofstream archivo;
  
  archivo.open("nordenados",ios::out); //abriendo el archivo
  
  if (archivo.fail()){
    cout<<"Error al crear el archivo";
    exit(1);
  }
  getline(cin,numeros);
  archivo<<numeros;
  archivo.close(); //cerrar archivo
  
  
  }
  
