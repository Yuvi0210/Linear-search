# Linear-search
#include <iostream>
using namespace std;

void Print_array(int * array , int n){
  for(int i = 0 ; i < n ; i++){
    cout<<array[i];
  }
}

int Linear_search(int * array , int n , int x){
  for(int i = 0 ; i < n ; i++ ){
    if(array[i] == x){
      return i;
      }
      else{
      return -1;
    }
}
    

int main (){
  int array[100];
  int n;
  cout<<"Enter the size of the array"<<endl;
  cin>>n;
  for(int i = 0; i < n ; i++){
    cin>>array[i];
    }
  cout<<Print_array(array , n)<<endl;
  int x;
  cout<<"Enter the number to be searched"<<endl;
  cin>>x;
  cout<<Linear_search(array , n , x)<<endl;
}  
