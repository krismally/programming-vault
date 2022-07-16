# Linked Lists Data Structure
## Definition
A sequential list of nodes that contain data and pointer to next node, always ends with null.

##### Where are they used?
1. Many list, stack, and queue implementations
2. Great for circular lists
3. Modeling real world objects (like train cars)
4. Seperate chaining for certain hash tables
5. In the emplimentation of adjacency lists for graphs

##### Important Terminology
- Head - 1st node in linked list
- Tail - Last node in linked list
- Pointer - Reference to another node
- Node - Object containing data and pointer(s)

#### Singly v. Doubly Linked Lists
- Singly linked lists...
	- Only hold reference to next node
	- Pros
		- Less memory
		- Simpler to implement
	- Cons
		- Can't easily access previous nodes
- Doubly linked lists...
	- Hold references to previous and next node
	- Pros
		- Can be traversed backwards
	- Cons
		- Double the memory of singly linked lists
- Both linked lists...
	- Contain refs to head and tail of the linked list for quick additions/removals

### Time Complexity 
#### Search
- Singly - O(n)
- Doubly - O(n)
#### Insert at head
- Singly - O(1)
- Doubly - O(1)
#### Insert at tail
- Singly - O(1)
- Doubly - O(1)
#### Remove at head
- Singly - O(1)
- Doubly - O(1)
#### Remove at tail
- Singly - O(n)
- Doubly - O(1)
#### Remove in middle
- Singly - O(n)
- Doubly - O(n)


## [[Implementation]]
