TODO run test and record running times for SIZE = 10, 100, 1000, 10000, ...

SIZE = 10 -> 234ms
SIZE = 100 -> 280ms
SIZE = 1000 -> 717ms
SIZE = 10000 -> 6s

 TODO Question: What conclusions can you draw about the performance of LinkedList vs. ArrayList when

linkedList -> 578ms
arrayList -> 389ms

testArrayListAddRemove() -> 416ms
testArrayListAccess() -> 253ms

testLinkedListAddRemove() -> 247ms
testLinkedListAccess() -> 525ms

from these tests you can see that ArrayList was slower compared to LinkedList when it came to
the AddRemove methods. Whereas, LinkedList was slower compared to ArrayList when it came
to the Access method.

This is because ArrayList has direct index access and so accessing is much faster compared to
LinkedList which has to iterate through each node in the list.

TODO Question: Also try with a LinkedList - does it make any difference?

for the TestList class switching from ArrayList and LinkedList had similar affects. LinkedList
turned out to have faster build time when it came to insertion and removing of objects.
Whereas ArrayList was faster when it came to indexing functions such as get and set.


TODO Question: What does this method do?

the .remove() method removes the element at the index specified in the parameter.
So .remove(5) would remove the 5th element

TODO Question: What does this one do?  list.remove(Integer.valueOf(5));

This method removes the element specified by the input at it's first occurance in the list.
So if there are multiple 5 in the list then it will remove the first one that is in the list

TODO Question: What happens if you use list.remove(Integer.valueOf(77))?

When changing it from i.remove to the one above, there is an error ConcurrentModificationException
causing the program to crash.


