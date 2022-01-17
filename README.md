# chef-and-fixed-deposits
#include <bits/stdc++.h>
#include<vector>
using namespace std;
int main()
{
	int t;
	cin>>t;
	while(t--)
	{
		int n,x;

		cin>>n>>x;
		int a[n];
		for(int i=0;i<n;i++)
		{
			cin>>a[i];
		}
		sort(a,a+n,greater<>());
		int sum=0,i;
		bool c=false;
		for(i=0;i<n;i++)
		{
			
			sum=sum+a[i];
			if(sum>=x)
			{
				c=true;
				break;
			}
		}
			if(c)
			{
				cout<<i+1<<endl;
			}
			else
			{
				cout<<"-1"<<endl;
			}

		}
	}

