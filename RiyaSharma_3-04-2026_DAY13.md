class Solution {
    public ListNode getIntersectionNode(ListNode headA, ListNode headB) {
        if (headA == null || headB == null) return null;
        ListNode pA = headA, pB = headB;
        
        while (pA != pB) {
            pA = pA == null ? headB : pA.next;
            pB = pB == null ? headA : pB.next;
        }
        return pA;
    }
}
<img width="1899" height="993" alt="{D24C6543-B104-46EB-95CF-4C1980118144}" src="https://github.com/user-attachments/assets/df504721-b145-49c4-9194-60d4d20f1b3f" />
