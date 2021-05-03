# Solution

```JavaScript :
var numWaterBottles = function(numBottles, numExchange) {
    if(numBottles < numExchange) {
        return numBottles
    }
    
    return numExchange + numWaterBottles(numBottles - numExchange + 1, numExchange)    
};
```
