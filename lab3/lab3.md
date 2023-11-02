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
## Part 2
