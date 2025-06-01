# C-_STL_Unordered_set

#include <bits/stdc++.h>
using namespace std;

int main() 
{   cout<<"hello"<<endl;

    unordered_set<int>i;
    
    i.insert(1);
    i.insert(1);
    i.insert(2);
    i.insert(1);
    i.insert(3);
    
    for(auto it=i.begin();it!=i.end();it++){
      cout<<* it<<" ";
    }cout<<endl;
    
    int n=2;
    //find sends the iterator of the value if found if not then send end iterator
    if(i.find(4)!=i.end()){
      cout<<"found";
    }
    else{
      cout<<"Not found"<<endl;
    }
    
    i.erase(i.begin());
    for(auto it=i.begin();it!=i.end();it++){
      cout<<* it<<" ";
    }cout<<endl;
    
    
    cout<<"size of unordered set="<<i.size()<<endl;
    
    i.clear();
    cout<<"size of unordered set="<<i.size()<<endl;
    
    
    return 0;
}
