# DS_notes-prac

## chap 1
information in memory 
- no exercises required for this chap
- dove into the basics of how we store data in our computer memory
- variables:
    - names representing the location of a piece of data in the computers memory
    - we can visualize memory as a long coloumn of bins 
    - double precision floating point number would require more memory, therefore more bins. ex, 12.34
    - boolean types, true or false
- composite data structures:
    - struct or an object, which gather multiple individual variables into a single group (list, array, dictionary)
    - good ex, buisness cards
    - we use the syntax composite.field to indicate accessing a particular field of a composite data structure (latest_record.name = "sublime blend")
- arrays
     - provide a simple mechanism for storing multiple values in adjacent or indexable bins (arr[3] = 4902)
     - the rows of lockers lining a school hallway
     - values inside the arrays are known as elements
     - arrays aren't like books on a shelf, you have to remove a book and place it somewhere else to replace that book 
        - to do this you can assign books to temporary values, move the elements inside, and then replace the element to the new open indexed space
- insertion sort
    - type of algo to sort values in an array
    - works by sorting a subset of the array and expanding this sorted range until the entire array is in order
    - coffee expiration data: compare the first two, from left to right, shortest expiration date to longest, and then uses that subset to file in the 3rd index into its rightful place. 
- strings
    - ordered lists, special kind of arrays
    - when we display a string on the screen, we are effectively iterating through each of its characters and displaying them one at a time
- why this matters 
    - staples of programming classes. 
    - very foundation of comp pro and data structures
    - concepts provide the baseline aganist which to evaluate dynamic data structures and thier impact on algorythms. 
    - dynamic data structure can offer trade-offs amoung efficency, flexibility and complexity. 

## chap 2 
binary search 
- checks the sorted list for a target value by repeated dividing the list in half, determining which of the two would contain the target value, discarding the other half
- linear scan 
    - providing a baseline for comparison for binary search 
    - works by testing each value in our list for our specific value
    - a single while loop iterates over each item in the array, the internal if statement compares that element to the target, as soon as we come across the element, it returns the element, if not, it will return -1 
    - brute force test garuenteed to find the itme of interest 
    - ex, going down the line of students asking each student their name till you find the one youre looking for 
- binary search algo
    - finds target value v in a sorted list, and only works on sorted data
    - algo can we written to work with data in either increasing or decreasing order
    - similar to logic when avoiding ice cream isle when we know we dont need ice cream. once we know an item isnt in a certain area, we can rule out that entire set of items 
    - searches the space between 2 bounds, the IndexHigh and the IndexLow, with IndexMid being the center of those two
        - IndexMid = Floor((IndexHigh + IndexLow) / 2)
    - we continue to cut the list in half until our value is found. 
    - binary search waits until the midpoint lands to our target value, because our search will only check the midpoint against out target 
- absent values 
    - if a value is not in the list, returns specified value in the algo
- implementing binary search 
    - implement binary search with a simple while loop
    - compute the mid point 
    - check the midpoint value aganist the target, if its a match we found our target
    - if the value is too high we adjsut our upper bounds 
- adapting binary search 
    - applying to books on a shelf, names in a phone book, clothing rack ordered by size 
    - instead of going value by value, binary search allows for better precision 
    - bisection search uses it to find the zero of a function, or the value of x such that f(x) = 0
- runtime
    - often analyze the runtime of an algo in terms of its average worse-case performance as the size of the data N grows
    - comp sci often use big O notation to more formally capture those concepts. 
    - we consider the same two aspects throughout for each algo
        - avergae case runtime of an algo as the size of the data grows 
        - worst case runtime of an algo as the size of the data grows
    - the benefit of needing only a longarithmic number of comparisons will far outwigh additional per steps costs

