class Solution {
public:
    bool judgeCircle(string moves) {
        int up =0;
        int right =0;
        for (int i=0;i<moves.size();i++){
            if (moves[i]== 'U'){
                up++;
            }

            else if (moves[i]== 'R'){
                right++;
            }

            else if (moves[i]== 'L'){
                right--;
            }

            else if (moves[i]== 'D'){
                up--;
            }
        }
        if(up==0 && right==0) return true;
        else return false;
    }
};
