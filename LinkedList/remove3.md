<div class="viewer">

### reverse3

<div>

Write a method reverse3 that reverses each successive sequence of 3 values in a list of integers. For example, suppose that a variable called list stores the following sequence of values:

    [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]

and we make the following call:

    list.reverse3();

Afterwards the list should store the following sequence of values:

    [3, 2, 1, 6, 5, 4, 9, 8, 7, 12, 11, 10, 15, 14, 13]

The first sequence of 3 values (1, 2, 3) has been reversed to be (3, 2, 1). The second sequence of 3 values (4, 5, 6) has been reverse to be (6, 5, 4). And so on. If the list has extra values that are not part of a sequence of 3, those values are unchanged. For example, if the list had instead stored:

    [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17]

The result would have been:

    [3, 2, 1, 6, 5, 4, 9, 8, 7, 12, 11, 10, 15, 14, 13, 16, 17]

Notice that the values (16, 17) are unchanged in position because they were not part of a sequence of three values.

These examples purposely used sequential integers to make the rearrangement clear, but you should not expect that the list will store sequential integers. For example, the following list:

    [3, 8, 19, 42, 7, 26, 19, -8, 193, 204, 6, -4, 99]

would be rearranged as follows:

    [19, 8, 3, 26, 7, 42, 193, -8, 19, -4, 6, 204, 99]

Your method should not change the list if it has fewer than three values.

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

You are writing a method that will become part of the LinkedIntList class. You may not call any methods of the class to solve this problem, you may not construct any new nodes, and you may not use any auxiliary data structure to solve this problem (no array, ArrayList, stack, queue, String, etc). You also may not change any data fields of the nodes. You MUST solve this problem by rearranging the links of the list.

</div>

</div>