class Solution {
    public ListNode middleNode(ListNode head) {
        ListNode slow = head;
        ListNode fast = head;

        while (fast != null && fast.next != null) {
            slow = slow.next;        // move 1 step
            fast = fast.next.next;   // move 2 steps
        }

        return slow;
    }
}
<img width="1920" height="984" alt="{867FE18C-3D1C-4305-A4AA-C65CC80623BD}" src="https://github.com/user-attachments/assets/f7e3bd97-d235-4346-a031-390f286b89f3" />
