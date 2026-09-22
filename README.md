# LeetCode 246 - Strobogrammatic Number

## Problem

Given a string representing a number, determine whether it is a strobogrammatic number.

A strobogrammatic number looks the same when rotated 180 degrees.

The valid digit rotations are:

```text
0 -> 0
1 -> 1
6 -> 9
8 -> 8
9 -> 6
```

## Example

### Input

```text
num = "69"
```

### Output

```text
true
```

### Example 2

```text
num = "88"
```

### Output

```text
true
```

### Example 3

```text
num = "962"
```

### Output

```text
false
```

## Approach

Use two pointers, one starting from the beginning and one from the end.

For every pair of digits, check whether rotating the left digit gives the right digit.

Valid pairs are:

```text
0 - 0
1 - 1
6 - 9
8 - 8
9 - 6
```

If any pair is invalid, return `false`.

## Algorithm

1. Create a mapping of valid rotated digit pairs.
2. Set two pointers at the beginning and end.
3. Compare the mapped left digit with the right digit.
4. If they do not match, return `false`.
5. Move both pointers toward the center.
6. Return `true` after all pairs are valid.

## Complexity

* Time Complexity: `O(n)`
* Space Complexity: `O(1)`

Where `n` is the number of digits.

## Language

Python

## LeetCode

Problem: 246 - Strobogrammatic Number

## Author

**T.Nandhini**
