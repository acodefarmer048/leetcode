# leetcode
4.07
class Solution:
    def twoSum(self, numbers: List[int], target: int) -> List[int]:
        left,right=0,len(numbers)-1
        while True:
            temp=numbers[left]+numbers[right]
            if temp>target:
                right-=1
            elif temp<target:
                left+=1
            else:
                return [left+1,right+1]
