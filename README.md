# Data-structure-practical-program-30
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

class LinkedList:
    def __init__(self):
        self.head = None

    def insert(self, data):
        new = Node(data)
        new.next = self.head
        self.head = new

    def display(self):
        temp = self.head
        while temp:
            print(temp.data, end=" ")
            temp = temp.next

l = LinkedList()
l.insert(10)
l.insert(20)
l.insert(30)

l.display()
30 20 10
