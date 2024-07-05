public class DoublyLinkedList<T> {
    private ListNode<T> head;

    public void listInsert(ListNode<T> x) {
        if (head == null) {
            head = x;
            return;
        }

        x.next = head;
        head.prev = x;
        head = x;
    }

    private static <T> void printList(ListNode<T> head) {
        ListNode<T> current = head;
        while (current != null) {
            System.out.print(current.key + " ");
            current = current.next;
        }
        System.out.println();
    }

    public static void main(String[] args) {
        DoublyLinkedList<Integer> list = new DoublyLinkedList<>();

        list.listInsert(new ListNode<>(1));
        list.listInsert(new ListNode<>(2));
        list.listInsert(new ListNode<>(3));
        list.listInsert(new ListNode<>(4));

        printList(list.head);
    }
}
