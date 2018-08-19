# python-notes

Inheritance in python:
  class X(object):
    def __init__(self, x):
      pass

    def doit(self, bar):
      pass

  class Y(X):
    def __init__(self):
      super(Y, self).__init__(123)

    def doit(self, foo):
      return super(Y, self).doit(foo)
      
      
Sorting in-place:
  data.sort(key=lambda tup: tup[1])
  
Sort using sort function and get a new list:
  sorted_by_second = sorted(data, key=lambda tup: tup[1])


Sorting objects:
  To sort the list in place...
  ut.sort(key=lambda x: x.count, reverse=True)

  To return a new list, use the sorted() built-in function...
  newlist = sorted(ut, key=lambda x: x.count, reverse=True)

Bitwise operators:

& Binary AND	Operator copies a bit to the result if it exists in both operands	(a & b) (means 0000 1100)
| Binary OR	It copies a bit if it exists in either operand.	(a | b) = 61 (means 0011 1101)
^ Binary XOR	It copies the bit if it is set in one operand but not both.	(a ^ b) = 49 (means 0011 0001)
~ Binary Ones Complement	It is unary and has the effect of 'flipping' bits.	(~a ) = -61 (means 1100 0011 in 2's complement form due to a signed binary number.
<< Binary Left Shift	The left operands value is moved left by the number of bits specified by the right operand.	a << 2 = 240 (means 1111 0000)
>> Binary Right Shift	The left operands value is moved right by the number of bits specified by the right operand.	a >> 2 = 15 (means 0000 1111)


Python List remove tricks:
del a[-1] - removes last element
del a[2:4] - removes the elements at index 2 and 3
a.pop(1)  - Removes the 1st element in the list

Other useful classes:
heapq, set, deque


