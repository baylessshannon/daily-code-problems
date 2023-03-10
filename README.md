# Daily Code Problems

This repo contians my solutions to different Daily Coding Problems. These problems are sent out daily to email subscribers and are meant to share common technical interview questions asked by large tech companies. The ratings (Easy, Medium, Hard) are provided in the email and are not necessarily a measure of personal difficulty.


For example, the first problem solved in this repo was asked by Google.

Given a list of numbers and a number ```k```, return whether any two numbers from the list add up to ```k```.

For example, given ```[10, 15, 3, 7]``` and ```k``` of ```17```, return true since ```10 + 7 is 17```.

My solution to this problem is contained in [problem-1.ipynb](https://github.com/baylessshannon/daily-code-problems/blob/master/problem-1.ipynb)

If you are interested in trying these problems yourself, sign up for the daily emails [here](https://www.dailycodingproblem.com/).

## Table of Contents

- [Problem 1 [Easy]](#problem-1)
- [Problem 2 [Hard]](#problem-2)
- [Problem 3 [Medium]](#problem-3)
- [Problem 4 [Hard]](#problem-4)
- [Problem 5 [Medium]](#problem-5)
- [Problem 6 [Hard]](#problem-6)
- [Problem 7 [Medium]](#problem-7)
- [Problem 8 [Easy]](#problem-8)
- [Problem 9 [Hard]](#problem-9)
- [Problem 10 [Medium]](#problem-10)
- [Problem 11 [Medium]](#problem-11)

## Problem 1

This problem was recently asked by Google.

Given a list of numbers and a number k, return whether any two numbers from the list add up to k.

For example, given [10, 15, 3, 7] and k of 17, return true since 10 + 7 is 17.

Bonus: Can you do this in one pass?

Find my solution [here](https://github.com/baylessshannon/daily-code-problems/blob/master/problem-01.ipynb)

## Problem 2 
This problem was asked by Uber.

Given an array of integers, return a new array such that each element at index i of the new array is the product of all the numbers in the original array except the one at i.

For example, if our input was [1, 2, 3, 4, 5], the expected output would be [120, 60, 40, 30, 24]. If our input was [3, 2, 1], the expected output would be [2, 3, 6].

Follow-up: what if you can't use division?

Find my solution [here](https://github.com/baylessshannon/daily-code-problems/blob/master/problem-02.ipynb)
## Problem 3
This problem was asked by Google.

Given the root to a binary tree, implement serialize(root), which serializes the tree into a string, and deserialize(s), which deserializes the string back into the tree.

For example, given the following Node class
```
class Node:
    def __init__(self, val, left=None, right=None):
        self.val = val
        self.left = left
        self.right = right
```
The following test should pass:
```
node = Node('root', Node('left', Node('left.left')), Node('right'))
assert deserialize(serialize(node)).left.left.val == 'left.left'
```


This problem is still a work in progress. See my work [here](https://github.com/baylessshannon/daily-code-problems/blob/master/problem-03.ipynb).

## Problem 4
This problem was asked by Stripe.

Given an array of integers, find the first missing positive integer in linear time and constant space. In other words, find the lowest positive integer that does not exist in the array. The array can contain duplicates and negative numbers as well.

For example, the input ```[3, 4, -1, 1]``` should give 2. The input ```[1, 2, 0]``` should give ```3```.

You can modify the input array in-place.

Find my solution [here](https://github.com/baylessshannon/daily-code-problems/blob/master/problem-04.ipynb)

## Problem 5
This problem was asked by Jane Street.

cons(a, b) constructs a pair, and car(pair) and cdr(pair) returns the first and last element of that pair. For example, car(cons(3, 4)) returns 3, and cdr(cons(3, 4)) returns 4.

Given this implementation of cons:
```
def cons(a, b):
    def pair(f):
        return f(a, b)
    return pair
```
Implement ```car``` and ```cdr```.

This problem is still a work in progress. See my work [here](https://github.com/baylessshannon/daily-code-problems/blob/master/problem-05.ipynb).

## Problem 6
This problem was asked by Google.

An XOR linked list is a more memory efficient doubly linked list. Instead of each node holding ```next``` and ```prev``` fields, it holds a field named ```both```, which is an XOR of the next node and the previous node. Implement an XOR linked list; it has an ```add(element)``` which adds the element to the end, and a ```get(index)``` which returns the node at index.

If using a language that has no pointers (such as Python), you can assume you have access to ```get_pointer``` and ```dereference_pointer``` functions that converts between nodes and memory addresses.

This problem is still a work in progress. See my work [here](https://github.com/baylessshannon/daily-code-problems/blob/master/problem-06.ipynb).

## Problem 7
This problem was asked by Facebook.

Given the mapping a = 1, b = 2, ... z = 26, and an encoded message, count the number of ways it can be decoded.

For example, the message '111' would give 3, since it could be decoded as 'aaa', 'ka', and 'ak'.

You can assume that the messages are decodable. For example, '001' is not allowed.

This problem is still a work in progress. See my work [here](https://github.com/baylessshannon/daily-code-problems/blob/master/problem-07.ipynb).

## Problem 8
This problem was asked by Google.

A unival tree (which stands for "universal value") is a tree where all nodes under it have the same value.

Given the root to a binary tree, count the number of unival subtrees.

For example, the following tree has 5 unival subtrees:
```
   0
  / \
 1   0
    / \
   1   0
  / \
 1   1
 ```

 This problem is still a work in progress. See my work [here](https://github.com/baylessshannon/daily-code-problems/blob/master/problem-08.ipynb).

 ## Problem 9
 This problem was asked by Airbnb.

Given a list of integers, write a function that returns the largest sum of non-adjacent numbers. Numbers can be 0 or negative.

For example, ```[2, 4, 6, 2, 5]``` should return ```13```, since we pick ```2```, ```6```, and ```5```. `[5, 1, 1, 5]` should return `10`, since we pick `5` and `5`.

Follow-up: Can you do this in O(N) time and constant space?

Find my solution [here](https://github.com/baylessshannon/daily-code-problems/blob/master/problem-09.ipynb).

 ## Problem 10
 This problem was asked by Apple.

Implement a job scheduler which takes in a function `f` and an integer `n`, and calls `f` after `n` milliseconds.

Find my solution [here](https://github.com/baylessshannon/daily-code-problems/blob/master/problem-10.ipynb).

## Problem 11
This problem was asked by Twitter.

Implement an autocomplete system. That is, given a query string `s` and a set of all possible query strings, return all strings in the set that have `s` as a prefix.

For example, given the query string de and the set of strings `[dog, deer, deal]`, return `[deer, deal]`.

Hint: Try preprocessing the dictionary into a more efficient data structure to speed up queries.

Find my solution [here](https://github.com/baylessshannon/daily-code-problems/blob/master/problem-11.ipynb).