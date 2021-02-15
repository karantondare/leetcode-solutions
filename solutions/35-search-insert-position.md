# Solution

```JavaScript :
var searchInsert = function(nums, target) {
    if(nums.includes(target)) {
        return nums.indexOf(target);
    } else {
      if (target > nums[nums.length - 1]) {
          nums.push(target);
        return nums.indexOf(target);
        }
       for(let i = 0; i < nums.length; i++) {
           if (target < nums[i]){
             nums.splice(i, 0, target);
        return nums.indexOf(target);
           }
       }
    }
};
```
