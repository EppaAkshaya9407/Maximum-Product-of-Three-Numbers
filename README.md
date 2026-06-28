# Maximum-Product-of-Three-Numbers
nums=list(map(int,input("Enter the numbers:").split()))
nums.sort()
n=len(nums)
if n==3:
    c=1
    for i in range(n):
        c*=nums[i]
    print(c)
else:
    r=nums[n-1]*nums[n-2]*nums[n-3]
    r=max(r,nums[0]*nums[1]*nums[n-1])
    print(r)
