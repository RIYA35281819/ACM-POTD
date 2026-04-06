class MyQueue {
    private Stack<Integer> incoming = new Stack<>();
    private Stack<Integer> outgoing = new Stack<>();
    
    public void push(int x) {
        incoming.push(x);
    }
    
    public int pop() {
        peek();
        return outgoing.pop();
    }
    
    public int peek() {
        if (outgoing.isEmpty()) {
            while (!incoming.isEmpty()) {
                outgoing.push(incoming.pop());
            }
        }
        return outgoing.peek();
    }
    
    public boolean empty() {
        return incoming.isEmpty() && outgoing.isEmpty();
    }
}
<img width="1920" height="977" alt="{E4679AE4-C802-4012-A9D7-EB19515FED65}" src="https://github.com/user-attachments/assets/ec5ea68e-9ebd-47e9-a9c7-8b2472c33e99" />
