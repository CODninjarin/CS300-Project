# CS300-Project
What was the problem you were solving in the projects for this course?

    ABCU was looking to create a program that would allow advisors to view students course plans. Initially different data structures were outlined using psuedocode and after an analysis, One data structure was chosen based on the analysis and code was created. After my analysis, I decided a Hash Table was the best data structure due to the runtime analysis showing it was a faster choice.
    
How did you approach the problem? Consider why data structures are important to understand.

    Though all the data structures perform similar tasks of holding objects and information, they do these differently, and with varying efficiency in both runtimes and code needed to complete a task. While a Vector is simple, it requires more steps to sort than a hashtable or tree, though they have the same worst case runtime. A main reason I chose a hash table for this project was because of the efficiency in searching/printing that it has over the other two structures. A vector requires a need to iterate over all of the objects within until the one needed is found, and the process is O(n^2). A tree would typically need to iterate over half of the tree at most, but if the tree happens to be unbalanced it could be a higher worst cas. it is at worst O(n), which is faster than a vector. A hash table has a search/print runtime of O(1), or constant time, because it does not require searching. The nodes are stored in a vector with their key being the index, so as long as you have the key you can instantly go to the node you need. With this function being an important part of the project, this difference made choosing a hashtable easy. 

How did you overcome any roadblocks you encountered while going through the activities or project?

    My biggest roadblock was within the code of the project. One of the features of a hash table is the act of hashing the key by dividing it by the total length of the table. Where I ran into issues with hashing the course ID because it contained letters as well as numbers. When converting a character to an int then back to a string, the character would go back to being a letter. I searched for ways to solve the issue and eventually figured out that to adjust a character from a letter to a number, the int had to be adjusted by 64 to match it's relative number in alphabetical order, ie. A = 1, B = 2, C = 3, etc. Numbers also needed to be adjusted by 48 since their int value and character value do not match. The resulting string was then converted to an int using the built in atoi function and then hashed.

How has your work on this project expanded your approach to designing software and developing programs?

    This project definitely shows the importance of trying different things to find what fits best. Understanding runtimes and the differences they can make is important, but also understanding what works best for different situations. I ran into a similar issue with another project recently where a CopyOnWriteArrayList was needed for information that was being modified within the list of a Java project. Choosing the right structures for a project is an important part of ensuring the project runs smoothly. This project also helped to understand how powerful of a tool pseudocode can be. 
    
How has your work on this project evolved the way you write programs that are maintainable, readable, and adaptable?

    I think the biggest thing was the use of pseudocode for multiple scenarios before deciding on one. I'm used to using psuedocode to plan a set project, but it was new to use it as a comparison tool. Using this could save time while creating a project due to less need to refactor if you decide to try something new. 

