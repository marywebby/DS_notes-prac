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