# big_mod

#include<bits/stdc++.h>
using namespace std;



#define		pb              push_back
#define		PB              pop_back
#define		nn              "\n"
#define		all(p)          p.begin(),p.end()
#define		zz(v)           v.size()
#define		ss              ' '
#define		pp              cout<<
#define 	S(a)            scanf("%lld",&a)
#define 	SS(a,b)         scanf("%lld %lld",&a,&b)
#define 	SSS(a,b,c)      scanf("%lld %lld %lld",&a,&b,&c)
#define		gcd(a,b)        __gcd(a,b)
#define		lcm(a,b)        (a*b)/gcd(a,b)
#define		pi              acos(-1.0)
typedef		long long       ll;
typedef		vector<ll>      vll;

ll bigMod(ll a,ll b,ll c)
{
    ll x,y;
    if (b==0)
        return 1;
    else if (b%2==0)
    {
      x=bigMod(a,b/2,c);
        return (x*x)%c;
    }
    else
    {
        y=a%c;
        x=bigMod(a,b-1,c);
        return (x*y)%c;
    }
}


int main()
{

    ll a,b,c=0,i=0,j=0,t,k,m,mx=0,n,x=0,y,z,ar[1005]={0};

    cin>>a>>b>>c;
    pp bigMod(a,b,c);

    
	printf("%d\n",fact);




    return 0;
}


