# move-zeroes-to-the-end
code
#include<iostream>
using namespace std;

void func(int arr[],int n){
    int count=0;
    for(int i=0;i<n;i++){
        if(arr[i]!=0){
          swap(arr[i],arr[count]);
          count++;
          
        }
    }
}

int main(){
    int n;
    cout<<"enter the size of array:"<<endl;
    cin>>n;
    int arr[n];
    cout<<"the given array:"<<endl;
    for(int i=0;i<n;i++){
    cin>>arr[i];
    }
    func(arr,n);
    cout<<"the required array is:"<<endl;
    for(int i=0;i<n;i++){
        cout<<arr[i]<<" ";
    }
}
