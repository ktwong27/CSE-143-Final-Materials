<div class="viewer">

### reOrder

<div>

Write a method of the LinkedIntList class called reOrder that assumes the list starts by being sorted by absolute value and reorders the list so that it is sorted by value. The resulting list should contain all the values from the original list in sorted order from smallest to greatest. For example, if the variable list stores the following:

    list = [0, -3, 9, 12, -13, -22, 43, 54]

The call of list.reOrder(); would change the list to store the following values:

    list = [-22, -13, -3, 0, 9, 12, 43, 54]

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

You are writing a method that will become part of the LinkedIntList class. You may define private helper methods to solve this problem, but otherwise you may not assume that any particular methods are available. You are allowed to define your own variables of type ListNode, but you may not construct any new nodes, and you may not use any auxiliary data structure to solve this problem (no array, ArrayList, stack, queue, String, etc). You also may not change any data fields of the nodes. You MUST solve this problem by rearranging the links of the lists. Your solution must run in O(n) time where n is the length of the list. As in the examples above, assume that the list starts sorted by absolute value.

</div>

</div>