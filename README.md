# Reverse String

Write a function that reverses a string. The input string is given as an array of characters `s`.

### Example:

**_Input:_** `s = ["h","e","l","l","o"]`

**_Output:_** `["o","l","l","e","h"]`

### Constraints:

`1 <= s.length <= 10^5`

`s[i] is a printable ascii character.`
 

### Follow up: 

Do not allocate extra space for another array. You must do this by modifying the input array in-place with O(1) extra memory.

## Solution in JavaScript:

```
var reverseString = function(s) {
    for (let i = 0; i < s.length / 2; i++) {
        let temp = s[i]
        s[i] = s[s.length - 1 - i]
        s[s.length - 1 - i] = temp
    }
};
```
