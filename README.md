# hello-world
#include <iostream>
using namespace std;
int binary(int b){
    int a[100],i=0,j,count[100],t,p;
    	while(b>0){
	    a[i]=b%2;
	    b=b/2;
	    i++;
	}
	
	
    
           
        int c=0;
        for(j=i-1;j>=0;j--){
            if(a[j]==1)
            c++;
            
        }
        for(t=0;t<i-1;t++){
            count[t]=c;
        }
        for(p=0;p<=t;p++){
            cout<<count[p];
        cout<<endl;
        }
        
}

int main() {
	int n,k,d[100];
	cin>>n;
	for(k=0;k<n;k++){
	    cin>>d[k];
	}
	for(k=0;k<n;k++){
	binary(d[k]);    
	}
	
	
	return 0;
}
