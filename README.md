# LeetCode
Problems and solutions in LeetCode.  
For more detailed solutions, please visit my blog: [Nightonke's Blog](http://blog.csdn.net/u012925008).  
Or wanna ask anything, my email is: Nightonke@outlook.com.

##Catalogue
|#    |Title                                        |Problem                              |Solution                                  |
|:----|:--------------------------------------------|:------------------------------------|:-----------------------------------------|
|1    |[Two Sum](https://leetcode.com/problems/two-sum/)|[_0001_Two_Sum.jpg](https://github.com/Nightonke/LeetCode/blob/master/leetcode/problems/_0001_Two_Sum.jpg)|[_0001_Two_Sum.h](https://github.com/Nightonke/LeetCode/blob/master/leetcode/solutions/_0001_Two_Sum.h)
|
|2|[Add Two Numbers](https://leetcode.com/problems/add-two-numbers/)|[_0002_Add_Two_Numbers.jpg](https://github.com/Nightonke/LeetCode/blob/master/leetcode/problems/_0002_Add_Two_Numbers.jpg)|[_0002_Add_Two_Numbers.h](https://github.com/Nightonke/LeetCode/blob/master/leetcode/solutions/_0002_Add_Two_Numbers.h)
|
|3|[Longest Substring Without RepeatingCharacters](https://leetcode.com/problems/longest-substring-without-repeating-characters/)|(_0003_Longest_Substring_Without_Repeating_Characters.jpg)[https://github.com/Nightonke/LeetCode/blob/master/leetcode/problems/_0003_Longest_Substring_Without_Repeating_Characters.jpg]|(_0003_Longest_Substring_Without_Repeating_Characters.h)[https://github.com/Nightonke/LeetCode/blob/master/leetcode/solutions/_0003_Longest_Substring_Without_Repeating_Characters.h]
|
|4|[Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring/)|[_0004_Median_of_Two_Sorted_Arrays.jpg](https://github.com/Nightonke/LeetCode/blob/master/leetcode/problems/_0004_Median_of_Two_Sorted_Arrays.jpg)|[_0004_Median_of_Two_Sorted_Arrays.h](https://github.com/Nightonke/LeetCode/blob/master/leetcode/solutions/_0004_Median_of_Two_Sorted_Arrays.h)
|
|5|[Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring/)|[_0005_Longest_Palindromic_Substring.jpg](https://github.com/Nightonke/LeetCode/blob/master/leetcode/problems/_0005_Longest_Palindromic_Substring.jpg)|[_0005_Longest_Palindromic_Substring.h](https://github.com/Nightonke/LeetCode/blob/master/leetcode/solutions/_0005_Longest_Palindromic_Substring.h)
|




##Tags
|#    |Tag                                          |Problems                             |               
|:----|:--------------------------------------------|:------------------------------------|
|1    |Array|Two Sum, Median of Two Sorted Arrays|   
|2    |Hash Table|Two Sum, Longest Substring Without Repeating Characters|
|3    |Linked List|Add Two Numbers|
|4    |Math|Add Two Numbers|
|5    |Two Pointers|Longest Substring Without Repeating Characters|
|6    |String|Longest Substring Without Repeating Characters, Longest Palindromic Substring|
|7    |Binary Search|Median of Two Sorted Arrays|
|8    |Divide and Conquer|Median of Two Sorted Arrays|
|9    |Dynamic Programming||
|10    |Backtracking||
|11    |Stack||
|12    |Heap||
|13    |Greedy||
|14    |Sort||
|15    |Bit Manipulation||
|16    |Tree||
|17    |Depth-first Search||
|18    |Breadth-first Search||
|19    |Graph||
|20    |Topological||
|21    |Trie||
|22    |Binary Search Tree||
|23    |Recursion||
|24    |Union Find||
|25    |Design||
|26    |Segment Tree||
|27    |Binary Indexed Tree||


##Intro
LeetCode is a awesome online judge where there are hundreds of programming problems for interview. 
So I record the problems(for some are not free) and solutions.
There are 2 dictionaries in the LeetCode project.  
  
|--problems  
|--solutions  
  
Problems dictionary for problems picture, for instance, _0001_Two_Sum.jpg.  
Solutions dictionary for solutions in C++ class, for instance, _0001_Two_Sum.h.  

##Solution Example
For instance, in _0001_Two_Sum.h, the structure is:  

```
//
// Created by 伟平 on 2015/11/23.
//

#ifndef LEETCODE__0001_TWO_SUM_H
#define LEETCODE__0001_TWO_SUM_H

class _0001_Two_Sum {

    class Solution {
    public:
        vector<int> twoSum(vector<int> & nums, int target) {
            unordered_map<int, int> m;
            int size = nums.size();
            for (int i = 0; i < size; i++) {
                unordered_map<int, int>::iterator j = m.find(target - nums[i]);
                if (j != m.end()) {
                    vector<int> answer;
                    answer.push_back(j->second + 1);
                    answer.push_back(i + 1);
                    return answer;
                }
                else {
                    m[nums[i]] = i;
                }
            }
        }
    };

};

#endif //LEETCODE__0001_TWO_SUM_H
```
Notice that the Solution class is the class which I submit in LeetCode.

##Solution Example
![_0001_Two_Sum.jpg](https://github.com/Nightonke/LeetCode/blob/master/leetcode/problems/_0001_Two_Sum.jpg)

License
--------

    Copyright 2015 Weiping Huang.

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
