#include<algorithm>
#include<iostream>
#include<string.h>
#include<limits.h>
using namespace std;

int main()
{
    int k;
    scanf("%d",&k);
    while(k--)
    {
        long long  int n;
        scanf("%lld",&n);
        long long int arr[n];
        for(long long int i = 0;i < n;i++)
        {
                scanf("%lld",&arr[i]);
        }
        sort(arr,arr+n);
        long long int min = arr[0];
        cout << (n-1)*min << endl;
    }
return 0;
}

