class Solution {
    public boolean isValid(String s) {
        Stack<Character> stack = new Stack<>();
        for (char c : s.toCharArray()) {
            if (c == '(' || c == '{' || c == '[') {
                stack.push(c);
            } else {
                if (stack.isEmpty()) return false;
                char top = stack.pop();
                if ((c == ')' && top != '(') || 
                    (c == '}' && top != '{') || 
                    (c == ']' && top != '[')) {
                    return false;
                }
            }
        }
        return stack.isEmpty();
    }
}

<img width="1920" height="980" alt="{8AC8C85D-0378-4C7D-A0F2-74E03BAE5233}" src="https://github.com/user-attachments/assets/b597ead6-68dc-48ae-9ade-ffc98128dcec" />
