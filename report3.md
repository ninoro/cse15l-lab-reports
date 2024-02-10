Lab Report 3 - Bugs and Commands (Week 5)
---
I chose the bug (`reverseInPlace`) from `ArrayExamples.java`. The buggy program was tested using `ArrayTests.java`

_Failure-inducing JUnit Test_:
```
@Test 
public void testReverseInPlace() {
    int[] input1 = {1, 2, 4};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{4, 2, 1}, input1);
}
```
_Not a failure-inducing JUnit Test_:
```
@Test
public void testReversed() {
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
}
```
_Screenshot of output while running these two tests_:
![Image](savedtest.png)
![Image](savedtest2.png)

_Before code change_:
```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
```
_After code change_:
```
 static void reverseInPlace(int[] arr) {
    for (int i = 0; i < arr.length / 2; i++) {
        int var = arr[i];
        arr[i] = arr[arr.length - i - 1];
        arr[arr.length - i - 1] = var;
    }
}
```
_Fix_: In the corrected code, we only loop through half of the array's length because when we're reversing an array, we need to swap elements from both ends towards the middle. This approach ensures that we don't swap elements twice. We use a temporary variable to temporarily hold the value of one element while we move another element. This prevents the loss of data during the swapping process. We swap the element at the current index (i) with the element at the opposite index from the end of the array (arr.length - i - 1). This swapping continues until we've swapped all elements from one end to the other.








