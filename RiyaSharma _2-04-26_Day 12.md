public class Solution {
    public ListNode deleteDuplicates(ListNode head) {
        ListNode current = head;

        while (current != null && current.next != null) {
            if (current.val == current.next.val) {
                current.next = current.next.next;
            } else {
                current = current.next;
            }
        }

        return head;
    }
}







<img width="1913" height="981" alt="{75E884DB-DB66-41D3-8B07-E96769179441}" src="https://github.com/user-attachments/assets/bb54c8c0-fb91-43c2-91df-5d434a8d5920" />
