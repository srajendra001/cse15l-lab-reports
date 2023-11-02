# Lab 3
## Part 1
Failure-inducing test:
```
@Test
public void testReverseInPlace2() {
  int[] input = { 1, 2, 3 };
  ArrayExamples.reverseInPlace(input);
  assertArrayEquals(new int[] { 3, 2, 1 }, input);
}
```
Input that does not fail:
```
@Test 
public void testReverseInPlace() {
  int[] input1 = { 3 };
  ArrayExamples.reverseInPlace(input1);
  assertArrayEquals(new int[]{ 3 }, input1);
}
```
Symptom showing up after running the tests:
![Symptom](symptoms.png)
Before fixing the bug:
```
static void reverseInPlace(int[] arr) {
  for(int i = 0; i < arr.length; i += 1) {
    arr[i] = arr[arr.length - i - 1];
  }
}
```
After fixing the bug:
```
static void reverseInPlace(int[] arr) {
  for(int i = 0; i < arr.length/2; i += 1) {
    int temp = arr[i];
    arr[i] = arr[arr.length - i - 1];
    arr[arr.length - i - 1] = temp;
  }
}
```
The change fixes the issue because it makes it so two elements are being swapped rather than one element being changed to another element. Additionally, the loop only goes through half of the array since swapping while iterating through the second half of the array would just return it back to its original state.
## Part 2
