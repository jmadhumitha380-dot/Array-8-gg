# Array-8-gg
Practice program
class Solution:
    def findEquilibrium(self, arr):
        total = sum(arr)
        left_sum = 0

        for i in range(len(arr)):
            total -= arr[i]

            if left_sum == total:
                return i

            left_sum += arr[i]

        return -1
Output:
Input: 
arr[]
1 2 0 3
Your Output:
2
Expected Output:
2
