 #include <map>
#include <set>
#include <list>
#include <cmath>
#include <ctime>
#include <deque>
#include <queue>
#include <stack>
#include <string>
#include <bitset>
#include <cstdio>
#include <limits>
#include <vector>
#include <climits>
#include <cstring>
#include <cstdlib>
#include <fstream>
#include <numeric>
#include <sstream>
#include <iostream>
#include <algorithm>
#include <unordered_map>

using namespace std;



int main() {
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */ 
    vector<int> a(4),d(4,0);
     for(int i=0;i<4;i++){
         cin>>a[i];
         
     }
   
    for(int i=1;i<4;i++)
    {
        d[i]+=d[i-1]+a[i-1];
    }
    for(int i=0;i<3;i++)
    {
        cout<<"P"<<i+1<<" "<<"(WT="<<d[i]<<"), ";
    }
    cout<<"P"<<4<<" "<<"(WT="<<d[3]<<")";
    return 0;
}
