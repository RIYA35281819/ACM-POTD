public class Solution {
    public boolean hasCycle(ListNode head) {
        ListNode slow = head, fast = head;

        while (fast != null && fast.next != null) {
            slow = slow.next;
            fast = fast.next.next;

            if (slow == fast) return true;
        }

        return false;
    }
}
<img width="1920" height="978" alt="{0A3280B9-020D-4C30-B4D8-F113B94678B1}" src="https://github.com/user-attachments/assets/f0a74120-b362-4e16-a52d-3fdb11ee365d" />
