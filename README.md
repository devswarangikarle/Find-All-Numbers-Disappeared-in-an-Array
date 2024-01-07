# Find-All-Numbers-Disappeared-in-an-Array
Given an array nums of n integers where nums[i] is in the range [1, n], return an array of all the integers in the range [1, n] that do not appear in nums.   


class Solution:
    def findDisappearedNumbers(self, nums):
        n = len(nums)
        num_set = set(nums)
        result = []

        for i in range(1, n + 1):
            if i not in num_set:
                result.append(i)

        return result

solution = Solution()

nums1 = [4,3,2,7,8,2,3,1]
print(solution.findDisappearedNumbers(nums1)) 

nums2 = [1,1]
print(solution.findDisappearedNumbers(nums2))  
