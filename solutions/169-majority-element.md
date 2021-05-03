# Solution

```JavaScript :
var majorityElement = function(nums) {
    const elementsHash = {};
    
    for(let i = 0; i < nums.length; i++) {
        const num = nums[i];
        elementsHash[num] = elementsHash[num] + 1 || 1;
        if (elementsHash[num] > nums.length / 2) return num;
    }
};
```
