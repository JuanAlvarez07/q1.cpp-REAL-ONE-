#include <iostream>
using namespace std;

int gcd( int x, int y){
  int gcd;
  for(int i=1 ; i<=x && i<=y  ; i++){
    if( (x%i==0) && (y%i==0) ){
      gcd=i;
    }
  }
  return gcd;
}
int main(){
  int first, second;
  do{
  cout<<"Enter the POSITIVE first number: ";
  cin>>first;
  }while(first<0);
  do{
  cout<<"Enter the POSITIVE second number: ";
  cin>>second;
  }while(second<0);
  int y= gcd(first,second);

  cout<<"The greatest common denominador of the two number is: "<<y<<endl;
  return 0;
}
