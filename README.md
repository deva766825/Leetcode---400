Question 1 CPP
Minimum Number of Chairs in a Waiting Room
class Solution {
public:
    int minimumChairs(string s) {
        
        int ans=0;
        int cnt = 0;
        for(char c:s){
            if(c=='E'){
                cnt++;
            }
            else{
                cnt--;
            }
            ans = max(cnt,ans);
        }
        return ans;
    }
};

