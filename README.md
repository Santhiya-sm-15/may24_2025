# may24_2025
The problem that i solved today in leetcode

1.You are given a 0-indexed array of strings words and a character x.

Return an array of indices representing the words that contain the character x.

Note that the returned array may be in any order.

Code:
class Solution {
    public List<Integer> findWordsContaining(String[] words, char x) {
        List<Integer> res=new ArrayList<>();
        for(int i=0;i<words.length;i++)
        {
            if(words[i].contains(String.valueOf(x)))
                res.add(i);
        }
        return res;
    }
}
