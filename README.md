# OS-Project
Operating System Project with c++ 
#include<iostream>
using namespace std;

void sorting(int arr[],char name[]){
	int max=0,index=0;
	for(int i=0;i<10;i++){
		index=i;
		for(int j=i+1;j<10;j++){
			if(arr[j]>arr[index]){
				index=j;
			}
		}
			char n=name[i];
			name[i]=name[index];
			name[index]=n;
			int a=arr[i];
			arr[i]=arr[index];
			arr[index]=a;
	}
}
