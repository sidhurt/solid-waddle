# solid-waddle
 Enter the marks of the students and display highest and lowest marks of the class. Apply ‘Max’ and ‘Min’ functions to find out the maximum value and minimum value from the list of elements. Pass an array by reference to ‘Max’ and ‘Min’ function from main. Display maximum and minimum values in main function. 
#include<iostream>
using namespace std;
void print_max(int arr[5]);
void print_min(int arr[5]);
int main()
{
    int arr[5]={45,55,20,10,36};
    print_max(arr);
    print_min(arr);
}
void print_max(int arr[5])
{
    int maximum=arr[0];
    for (int i=0;i<5;i++)
    {
        if(maximum<arr[i])
        {
            maximum=arr[i];
        }
    }
    cout<<"The highest marks in the class are :"<<maximum<<endl;
}
void print_min(int arr[5])
{
    int minimum=arr[0];
    for(int i=0;i<5;i++)
    {
        if (minimum>arr[i])
        {
            minimum=arr[i];
        }
    }
    cout<<"The lowest marks in the class are:"<<minimum<<endl;
}
