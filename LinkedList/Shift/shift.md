<div class="viewer">

### shift

<div>

Write a method called shift that rearranges the elements of a list of integers by moving to the end of the list all values that are in even-numbered positions and otherwise preserving list order. For example, if you have a variable called list that stores the following:

    [0, 1, 2, 3, 4, 5, 6, 7]

then the call:

    list.shift();

should rearrange the list to be:

    [1, 3, 5, 7, 0, 2, 4, 6]

In this example the values in the original list were equal to their positions and there were an even number of elements, but that won't necessarily be the case. For example, if the list had instead stored:

    [4, 17, 29, 3, 8, 2, 28, 5, 7]

then after a call on shift it would store:

    [17, 3, 2, 5, 4, 29, 8, 28, 7]

Notice that it doesn't matter whether the value itself is odd or even. What matters is whether the value appears in an even index (index 0, 2, 4, etc). Also notice that the original order of the list is otherwise preserved.

You are writing a public method for a linked list class defined as follows:

    public class ListNode {
        public int data;       // data stored in this node
        public ListNode next;  // link to next node in the list

        <constructors>
    }

    public class LinkedIntList {
        private ListNode front;

        <methods>
    }

You are writing a method that will become part of the LinkedIntList class. You may define private helper methods to solve this problem, but otherwise you may not assume that any particular methods are available. You are allowed to define your own variables of type ListNode, but you may not construct any new nodes, and you may not use any auxiliary data structure to solve this problem (no array, ArrayList, stack, queue, String, etc). You also may not change any data fields of the nodes. You MUST solve this problem by rearranging the links of the list.

</div>

</div>