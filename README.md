# Replace-a-word
class Solution {
  public:
    string replaceAll(string str, string oldW, string newW) {
        // code here
        int n=oldW.size();
        string ans="";
        for(int i=0;i<str.size();i++){
            if(str.substr(i,n)==oldW){
                ans+=newW;
                i+=n-1;
            }
        
            else{
                ans+=str[i];
               
            }
        }
        return ans;
    }
};
