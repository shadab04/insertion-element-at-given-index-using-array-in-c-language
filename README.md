# insertion-element-at-given-index-using-array-in-c-language
int insert(int arr[],int size,int element,int index,int capacity)
{
    if(size>=capacity){
     return -1;
    }
    for(int i=size-1;i>=index;i--)
    {
        arr[i+1]=arr[i];
    }
    arr[index]=element;
}
*
{
    int arr[100]={5,6,9,10,20};
    int size=5,index=3;
    display(arr,size);
    deletion(arr,size,index,100);
    size=size-1;
    display(arr,size);
    return 0;
}
void display(int arr[],int n)
{
    for(int i=0;i<n;i++)
    {
        printf("\n%d",arr[i]);
    }
}
int deletion(int arr[],int size,int index)
{
    for(int i=index;i<size-1;i++)
    {
        arr[i]=arr[i+1];
    }
}
