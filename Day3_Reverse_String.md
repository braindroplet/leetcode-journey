
### Problem
```
Write a function that reverses a string. The input string is given as an array of characters s.
You must do this by modifying the input array in-place with O(1) extra memory.
```
### Examples
```
Input: s = ["h","e","l","l","o"]
Output: ["o","l","l","e","h"]
Example 2:

Input: s = ["H","a","n","n","a","h"]
Output: ["h","a","n","n","a","H"]
```

### Constraints
```
1 <= s.length <= 105
s[i] is a printable ascii character.
```

### Solution A
```
class Solution {
    public void reverseString(char[] s) {
        int standard = s.length/2;     
        int i = 0;
       while(i<standard){
           int reverseIndex = s.length-1- i;
            char temp = s[reverseIndex];
            s[reverseIndex] = s[i]; 
            s[i] = temp; 
            i++;
        }
    }
}
```

### Solution B

✨ 개선 포인트 (선택 사항)
1. standard 없이도 가능
standard = s.length / 2 를 굳이 변수로 만들지 않아도 i < s.length / 2로 직접 써도 깔끔해요.
→ 코드가 한 줄 더 줄어들고, 의미가 더 직관적해짐

2. for문으로 바꾸면 더 간결함
while 대신 for문을 쓰면 "초기화 + 조건 + 증감"이 한 줄에 들어가서 더 보기 좋아요
→ 동작은 동일, 하지만 코드 스타일이 더 깔끔해짐
```
for (int i = 0; i < s.length / 2; i++) {
    int reverseIndex = s.length - 1 - i;
    char temp = s[reverseIndex];
    s[reverseIndex] = s[i]; 
    s[i] = temp; 
}
```

3. 변수명 개선 (선택 사항)
기존 변수명	제안	이유
```
standard  ---> 생략 또는 mid	: 의미 전달이 조금 애매
reverseIndex  --->	j or right	: 짝이 되는 인덱스임을 직관적으로 표현 가능
```

### Interview Point
```
“Since the problem asked for an in-place reversal with constant space,
I used a two-pointer approach starting from both ends and swapping characters until they meet in the middle.
I used a for loop for clarity, and this ensures both readability and performance.”
```


