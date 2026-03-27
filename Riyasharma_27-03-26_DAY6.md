import java.util.HashSet;

class Solution {
    public boolean checkIfExist(int[] arr) {
        HashSet<Integer> set = new HashSet<>();
        
        for (int num : arr) {
            if (set.contains(2 * num) || (num % 2 == 0 && set.contains(num / 2))) {
                return true;
            }
            set.add(num);
        }
        
        return false;
    }
}
<img width="1919" height="982" alt="{84C586E3-CDA1-4ED1-B42B-21E0B36D3AA8}" src="https://github.com/user-attachments/assets/005f64ae-6fcf-47f5-aadf-eda631c82ff1" />
