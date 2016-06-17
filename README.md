#include <iostream>
using namespace std;

struct pila{

	char element;
	pila*siguiente;
};
pila* down=NULL;
pila* top=NULL;
char letter;
class pi {
public:
	void push(char letter);
	void pop();
	void top();
	void counter();
};
void pi::push(char letter){
down= new(pila);
down->element=letter;
down->siguiente=top;
top=down;

}

void pi::pop(){
pila = delete;
cout<<"pila"<<endl;
delete=top;
delete=NULL;
}

void pi::top(){
pila* mi=top;
if (top !=NULL){
cout<<"pile"<<mi->element<<endl;
}else{
	cout<<"no hay dato alguno"<<endl;
}
}
void pi::counter(){
	pila* aux=top;
	int k=0;
	while (aux !=NULL){
	aux=aux->siguiente;
	k=k+1;
	}
	cout<<"total de numeros en datos: \n" <<k<<endl;
	cout<<"\n\n"<<endl;
}

	return 0;
}
