class Solution {
    public ListNode reverseList(ListNode head) {
        ListNode prev = null;
        ListNode curr = head;
        
        while (curr != null) {
            ListNode next = curr.next;
            curr.next = prev;
            prev = curr;
            curr = next;
        }
        
        return prev;
    }
}
<img width="1903" height="913" alt="{9FA4777B-C5FF-438A-9409-584FEE056712}" src="https://github.com/user-attachments/assets/ee49193e-28d3-4860-9ade-ad408d6a5daa" />
