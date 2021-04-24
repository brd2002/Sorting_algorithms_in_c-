# Sorting_algorithms_in_c++
sortingAlgorithms
                          SORTaLGORITHMS
                          1. Selection Sort
                          2. Bubble Sort
                          3. Recursive Sort
   1.SELECTION_SORT
   ALGORITHMS   
   implemented in c++
    code:::
       #include<bits/stdc++.h>
using namespace std;
void swap(int *xp , int *yp)
{
    int temp = *xp;
    *xp = *yp;
    *yp = temp;
}
void selectionSort(int arr[] , int n )
{
    int i , j ,min_idx;
    for(i = 0 ;i<n-1;i++){
        min_idx = i;
         for(j =i+1 ;j<n ;j++)
            if(arr[j]<arr[min_idx])
            swap(&arr[min_idx] ,&arr[j]);
    }
}
void printarray(int arr[] , int size)
{
    int i;
    for(i =0 ;i<size ; i++)
        cout<< arr[i] << "  ";

}
int main()
{
    int arr[] = {1,4,2,3,7,6,5,9,8};
    int n = sizeof(arr)/sizeof(arr[0]);
    selectionSort(arr , n );
    cout<< "SortEd Array:";
    printarray(arr , n);
    return 0;
}


OUTPUT : 1,2,3,4,5,6,7,8,9

2.Bubble Sort
 ALGORITHMS implemented in c++
      #include<bits/stdc++.h>
using namespace std;
void swap(int *xp , int *yp)
{
    int temp = *xp;
    *xp = *yp;
    *yp = temp;
}
void bubbleSort(int arr[] , int n )
{
  int i,j;
  for(i = 0 ;i<n-1 ; i++)
  for(j = i+1 ;j<n-i-1;j++)
    if(arr[j]>arr[j+1])
    swap(&arr[j] ,&arr[j+1]);
}
void printarray(int arr[] , int size)
{
    int i;
    for(i =0 ;i<size ; i++)
        cout<< arr[i] << "  ";

}
int main()
{
    int arr[] = {1,4,2,3,7,6,5,9,8};
    int n = sizeof(arr)/sizeof(arr[0]);
    bubbleSort(arr , n );
    cout<< "SortEd Array:";
    printarray(arr , n);
    return 0;
}

OUTPUT: 1,2,3,4,5,6,7,8,9


3.Recursive Sort
ALGORITHMS implemented in c++
    #include<bits/stdc++.h>
using namespace std;
void swap(int *xp , int *yp)
{
    int temp = *xp;
    *xp = *yp;
    *yp = temp;
}
void recursiveSort(int arr[] , int n )
{
int i;
for(i = 0 ;i<n ; i++)
    if(arr[i]>arr[i+1])
    swap(&arr[i],&arr[i+1]);
}
void printarray(int arr[] , int n)
{
    int i;
    for(i =0 ;i<n ; i++)
        cout<< arr[i] << "  ";

}
int main()
{
    int arr[] = {1,4,2,3,7,6,5,9,8};
    int n = sizeof(arr)/sizeof(arr[0]);
    recursiveSort(arr , n );
    cout<< "SortEd Array:";
    printarray(arr , n);
    return 0;
}
 
 
 OUTPUT : 1,2,3,4,5,6,7,8,9
 
 
 // CODE WITH BRD007


