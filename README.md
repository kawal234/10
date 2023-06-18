# 10
#include<iostream>
#include<vector>// For using vector datatype
using namespace std;


// vectors in C++
// this is a dynamic arrays--> resize when insert/ delete elements 
// Memory allocation is Contiguous in Nature

//syntax
// int main(){
//     vector<int> v;// for initialing a vector
//     v.size();// to find the size of the vector
//     v.resize(8); // by this we can resize the vector size
//     v.capacity();// this is the capacity of the vector(capacity>= size)
//     // Capacity 2^n ke terms meh increase hoti h(compiler dependent bhi hota h)
//     v.push_back(3);// to add elememts in V to the last
//    // v.insert(1,29); // this is used to insert a certain position and element 
//     v.begin();// this occupy the first element
//     v.end();// this occupy the last element
//     v.pop_back(); // this deletes the last element of the array
//     //v.erase(2);// deletes the elemnt given>> position of the element is given
//     v.clear();// to delete whole array

//     return 0;
// }


// Lopping in Vectors 

// int main(){
//     vector<int> v;
//     // for loop
//     for(int i=0;i<5;i++){
//         int el;
//         cin>>el;
//         v.push_back(el);
//     }
//     for(int i=0;i<v.size();i++){
//         cout<<v[i]<<" ";

//     }
//     cout<<endl;
//     v.insert(v.begin()+2,6);

//     // for each loop
//     for(int e:v){
//         cout<<e<<" ";
//     }
//     cout<<endl;

//     v.erase(v.end()-2);
//     // while loop

//     int idx = 0;
//     while(idx<v.size()){
//         cout<<v[idx++]<<" ";
//     }
//     return 0;
// }


// Problem 1- to find the last occurence of the array

// int main(){
//     vector<int> v(6);
//     for(int i=0;i<6;i++){
//         cin>>v[i];
//     }
//     cout<<"Enter x:";
//     int x;
//     cin>>x;

//     for(int i=v.size()-1;i>=0;i--){
//         if(v[i]==x){
//             cout<<"Last Occurance at index : "<<i+1<<"\n";
//             break;
//         }
//     }
//     return 0;
// }


// Problem 2- to count number of occurences of a particular element X

// int main(){
//     vector<int> v(6);
//     for(int i=0;i<6;i++){
//         cin>>v[i];
//     }
//     cout<<"Enter x:";
//     int x;
//     cin>>x;

//     for(int i=0;i<v.size();i++){
//         if(v[i]==x){
//             cout<<"Last Occurance at index : "<<i+1<<"\n";
//         }
//     }
//     return 0;
// }


// Problem 3 - to check is the array is sorted or not

// int main(){
//     int arr[] = {1,2,3,4,5,6};
    
//     bool sorted = true;
//     for(int i=1;i<6;i++){
//         if(arr[i]<=arr[i-1]){
//             sorted = false;
//         }
//     }
//     cout<<sorted<<endl;
//     return 0;
// }


// Problem 4 - find difference between sum of elements at even indices and sum of elements at odd indices

int main(){
    int arr[] = {1,2,3,4,5,6};
    int answersum = 0;
    for(int i=0;i<6;i++){
        if(i%2==0){
            answersum+=arr[i];
        }
        else{
            answersum-=arr[i];
        }
    }
    cout<<answersum<<endl;
    return 0;
}

  
