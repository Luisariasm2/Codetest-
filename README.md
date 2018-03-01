# Codetest-
Prueba de Codigo 
unsigned char flags =1,flags_=127 ,tost = 1, micro =2, luces =4, refrigerador=8, cafetera=16,  licuadora=32, horno = 64;
int opcion =0,seleccion=0,seleccion_n=0,a=0,b=0,c=0;
char confirmacion =0;
int fla_gs=0,total;


using namespace std;

int main(){
	
	do{
	
	cout<<"Seleccione la opcion que desea :\n"<<endl;
	cout<<"1. Encender Electrodomesticos "<<endl;
	cout<<"2. Apagar Electrodomesticos "<<endl;
	cout<<"3. Encender lo que esta apagado y apagar lo que esta encendido "<<endl;
	cout<<"4. Consumo total en watts"<<endl;
	cout<<"5. salir del programa"<<endl;
	cin>>opcion;
	
	switch(opcion){
		case 1:
			do{
			system("cls");
			cout<<"lista de Electrodomesticos que desea encender"<<endl;
			cout<<" 1.tostadora \n 2.microondas \n 3.luces \n 4.refrigerador \n 5.cafetera \n 6.licuadora \n 7.horno \n 8.todos los electrodomesticos \n 9.salir"<<endl;
			cin>>seleccion;
			switch(seleccion){
			
				case 1:
					system("cls");
					cout<<"1. Desea encender tostadora [s/n] "<<endl;
					cin>>confirmacion;
					if( confirmacion == 's' ){	
						flags= flags | tost;
						cout<<"Tostadora esta encendida"<<endl;
						}
					else{
					cout<<"tostadora esta apagada"<<endl;
						}
					system("pause");
						break;
				
				case 2:
					system("cls");
					cout<<"Desea encender Microondas [s/n] "<<endl;
					cin>>confirmacion;
					if( confirmacion == 's' ){
					flags= flags | micro;
					cout<<"Microondas esta encendida"<<endl;
					}
					else{
					cout<<"Microondas esta apagada"<<endl;
					}
					system("pause");
					break;
					
				case 3:
					system("cls");
					cout<<"Desea encender Luces [s/n] "<<endl;
					cin>>confirmacion;
					if( confirmacion == 's' ){
					flags= flags | luces;
					cout<<"Luces esta encendida"<<endl;
					}
					else{
					cout<<"Luces esta apagada"<<endl;
					}
					system("pause");
					break;
				
				case 4:
					system("cls");
					cout<<"Desea encender refrigerador [s/n] "<<endl;
					cin>>confirmacion;
					if( confirmacion == 's' ){
					flags= flags | refrigerador;
					cout<<"refrigerador esta encendida"<<endl;
					}
					else{
					cout<<"refrigerador esta apagada"<<endl;
					}
					system("pause");
					break;
					
				case 5:
					system("cls");
					cout<<"Desea encender cafetera [s/n] "<<endl;
					cin>>confirmacion;
					if( confirmacion == 's' ){
					flags= flags | cafetera;
					cout<<"cafetera esta encendida"<<endl;
					}
					else{
					cout<<"cafetera esta apagada"<<endl;
					}
					system("pause");
					break;
					
				case 6:
					system("cls");
					cout<<"Desea encender licuadora [s/n] "<<endl;
					cin>>confirmacion;
					if( confirmacion == 's' ){
					flags= flags | licuadora;
					cout<<"licuadora esta encendida"<<endl;
					}
					else{
					cout<<"licuadora esta apagada"<<endl;
					}
					system("pause");
					break;
					
				case 7:
					system("cls");
					cout<<"Desea encender horno [s/n] "<<endl;
					cin>>confirmacion;
					if( confirmacion == 's' ){
					flags= flags | horno;
					cout<<"horno esta encendida"<<endl;
					}
					else{
					cout<<"horno esta apagada"<<endl;
					}
					system("pause");
					break;
				case 8:
					system("cls");
					cout<<"Desea encender todos los electrodomestidos[s/n]"<<endl;
					cin>>confirmacion;
					if (confirmacion== 's'){
					flags = flags_ | horno | licuadora |cafetera | refrigerador | luces | tost| micro;
					cout<<"Todos los electrodomesticos estan encendidos"<<endl;
					}
					else {
						cout<<"Todos los electrodomesticos estan apagados"<<endl;
					}
					system("pause");
					break;	
				case 9:
					system("cls");
					break;}
			}while(seleccion!=9);
			break;
			
		case 2:
			do{
			system("cls");
			cout<<"Lista de lectrodomesticos que desea apagar"<<endl;
			cout<<" 1.tostadora \n 2.microondas \n 3.luces \n 4.refrigerador \n 5.cafetera \n 6.licuadora \n 7.horno \n 8.apagar todos los electrodomesticos \n 9.salir"<<endl;
			cin>>seleccion_n;
			switch(seleccion_n){
				case 1:
					system("cls");
					cout<<"Desea apagar tostadora [s/n] "<<endl;
					cin>>confirmacion;
					if( confirmacion =='s' ){
					flags = flags &~tost;
					cout<<"tostadora esta apagado"<<endl;
					}
					else{
					cout<<"tostadora esta encendida"<<endl;
					}
					system("pause");
					break;
				case 2:
					system("cls");
					cout<<"Desea apagar microondas [s/n] "<<endl;
					cin>>confirmacion;
					if( confirmacion =='s' ){
					flags = flags &~micro;
					cout<<"microondas esta apagado"<<endl;
					}
					else{
					cout<<"microondas esta encendida"<<endl;
					}
					system("pause");
					break;	
				case 3:
					system("cls");
					cout<<"Desea apagar luces [s/n] "<<endl;
					cin>>confirmacion;
					if( confirmacion =='s' ){
					flags = flags &~luces;
					cout<<"luces esta apagado"<<endl;
					}
					else{
					cout<<"luces esta encendida"<<endl;
					}
					system("pause");
					break;
				case 4:
					system("cls");
					cout<<"Desea apagar refrigerador[s/n] "<<endl;
					cin>>confirmacion;
					if( confirmacion =='s' ){
					flags = flags &~refrigerador;
					cout<<"refrigerador esta apagado"<<endl;
					}
					else{
					cout<<"refrigerador esta encendida"<<endl;
					}
					system("pause");
					break;
				case 5: 
					system("cls");
					cout<<"Desea apagar cafetera[s/n] "<<endl;
					cin>>confirmacion;
					if( confirmacion =='s' ){
					flags = flags &~cafetera;
					cout<<"cafetera esta apagado"<<endl;
					}
					else{
					cout<<"cafetera esta encendida"<<endl;
					}
					system("pause");
					break;
				case 6:
					system("cls");
					cout<<"Desea apagar licuadora[s/n] "<<endl;
					cin>>confirmacion;
					if( confirmacion =='s' ){
					flags = flags &~licuadora;
					cout<<"licuadora esta apagado"<<endl;
					}
					else{
					cout<<"licuadora esta encendida"<<endl;
					}
					system("pause");
					break;
				case 7:
					system("cls");
					cout<<"Desea apagar el  horno[s/n] "<<endl;
					cin>>confirmacion;
					if( confirmacion =='s' ){
					flags = flags &~horno;
					cout<<"horno esta apagado"<<endl;
					}
					else{
					cout<<"horno esta encendida"<<endl;
					}
					system("pause");
					break;
				case 8:
					system("cls");
					cout<<"Desea apagar todos los electrodomesticos [s/n] "<<endl;
					cin>>confirmacion;
					if( confirmacion =='s' ){
					flags = flags &~(horno |licuadora |cafetera |refrigerador | luces | tost | micro);
					cout<<"todos los electrodomesticos estan apagado"<<endl;
					}
					else{
					cout<<"todos los electrodomesticos estan encendida"<<endl;
					}
					system("pause");
					break;
				case 9:
					system("cls");
					break;}
				}while(seleccion_n!=9);
				break;
		case 3:
			system("cls");
			cout<<"Desea Encender lo que esta apagado y apagar lo que esta encendido [s/n]"<<endl;
			cin>>confirmacion;
			if( confirmacion =='s' ){
				 if((flags&micro)==micro){
					flags=flags&~micro;
					cout<<"se apago el microondas"<<endl;
				}
				else {
					flags=flags | micro;
					cout<<"se prendio la  micro"<<endl;
					}
				if ((flags&tost)==tost){
					flags=flags&~tost;
					cout<<"se apago la tostadora"<<endl;
				}
				else{
						flags=flags | tost;
					cout<<"se prendio la  tostadora"<<endl;
					
				}
				if ((flags&(luces))==luces){
					flags=flags&~luces;
					cout<<"se apago el luces"<<endl;
				}	
				else{
					flags=flags | luces;
					cout<<"se prendio la luces"<<endl;
				}
				if((flags&(refrigerador))==refrigerador){
					flags=flags&~refrigerador;
					cout<<"se apago el refrigerador"<<endl;
				}	
				else{
					flags=flags | refrigerador;
					cout<<"se prendio la refrigerador"<<endl;
				}
				if((flags&(cafetera))==cafetera){
					flags=flags&~cafetera;
					cout<<"se apago el cafetera"<<endl;
				}
				else {
					flags=flags | cafetera;
					cout<<"se prendio la cafetera"<<endl;
				}
				if((flags&(licuadora))==licuadora){
					flags=flags&~licuadora;
					cout<<"se apago el licuadora"<<endl;
				}
				else {
					flags=flags | licuadora;
					cout<<"se prendio la licuadora"<<endl;
				}
				if((flags&(horno))==horno){
					flags=flags&~horno;
					cout<<"se apago el horno"<<endl;
				}
				else{
					flags=flags | horno;
					cout<<"se prendio la horno"<<endl;
				}	
				system("pause");
				}	
				
				break;
		case 4:
			system("cls");
			cout<<"consumo total:"<<endl;
			if((flags & tost)==tost){
				total=total+800;}
			else{
				total=total;
			}
			if((flags & micro)==micro){
				total=total+1000;}
			else{
				total=total;
				}
			if((flags &luces )==luces){
				total=total+40;}
			else{
				total=total;
				}
			if((flags &refrigerador )==refrigerador){
				total=total+300;}
			else{
				total=total;
				}
			if((flags &cafetera )==cafetera){
				total=total+800;}
			else{
				total=total;
				}	
			if((flags &licuadora )==licuadora){
				total=total+300;}
			else{
				total=total;
				}	
			if((flags &horno )==horno){
				total=total+1200;}
			else{
				total=total;
				}		
				cout<<"El consumo total es :"<<total<<endl;
				break;
		case 5:
			system("cls");
			break;
		}
			}while( opcion !=10);
		
	return 0;
}
