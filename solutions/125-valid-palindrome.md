# Solution

```JavaScript :
var isPalindrome = function(s) {
   const san = s.replace(/[^a-zA-Z0-9]/g, "").toLowerCase();
    return san.split("").reverse().join("") == san;
};
```
