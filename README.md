# bubble-sort

#include <iostream>
using namespace std;

void sortarray(int arr1[]){
    int i , j , temp;

    for(int i=0; i<4; i++){
        for(j=i+1; j<5; j++){
            if(arr1[i]>arr1[j]){
                temp = arr1[i];
                arr1[i] = arr1[j];
                arr1[j] = temp;
            }
        }
    }
    cout << "\nSorted array: {";
    for(int i=0; i<5; i++){
        cout << arr1[i] << " , ";
    }
    cout << "\b\b}";

}

int main(){
    int arr[5];
    cout << "Enter 5 integers: ";
    for(int i=0;i<5;i++){
        cin>>arr[i];
    }
    cout << "Unsorted array: {";
    for(int i=0; i<5; i++){
        cout << arr[i] << " , ";
    }
    cout << "\b\b}";
    cout << "";

    sortarray(arr);
    return 0;
}
