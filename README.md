### Task 8kyu:
You will be given an array a and a value x. All you need to do is check whether the provided array contains the value.

Array can contain numbers or strings. X can be either.
Return true if the array contains the value, false if not.

[Task link](https://www.codewars.com/kata/57cc975ed542d3148f00015b/java)

#### Solution: 
```Java
public class solution {
    public static boolean check(Object[] arr, Object value) {
        for (int i = 0; i < arr.length; i++) {
            if (arr[i].equals(value)) return true;
        }
        return false;
    }
}
```

#### Fav solution: 
```Java
import java.util.Arrays;

public class Solution {

    public static boolean check(Object[] a, Object x) {
        return Arrays.asList(a).contains(x);
    }

}
```

### Task 7kyu:
You've just moved into a perfectly straight street with exactly n identical houses on either side of the road. Naturally, you would like to find out the house number of the people on the other side of the street. 
[Task link](https://www.codewars.com/kata/5f0ed36164f2bc00283aed07/java)

#### Solution:
```Java
public class Codewars2 {
    public static void main(String[] args) {

    }
    public static long overTheRoad(long address, long n) {
        long inv = 1 + n * 2;
        return inv-address;
    }
}
```
#### Fav solution:
I liked this binary shift multiplying.
```Java
class CodeWars {
  public static long overTheRoad(long a, long n) {
    return (n<<1) - --a;
  }
}
```


