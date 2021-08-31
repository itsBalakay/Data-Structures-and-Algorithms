Data Structures and Algorithms #1 - What are Data Structures ? (CS Dojo)

Data structures === different ways to store stuff on your computer.

As example: map system for plaza

    Could use:
        Lists.... ex (Home, Store A); (Store A, Home); (Home, Intersection);
            You can't go from Store A to Intersection because there is no (Store A, Intersection) in the list. === Array or list data structure

        Table like list : | Home | (Store A, Store B, Intersection) | == all the places you could go on the right === Hash table data structure

Algorithms === operations you can perform on different data structures + sets of instructions for executing them

    to understand algorithms in the previos map system example : it is very simple to figure it out by looking at it so you must write it in terms that a computer will understand.

        Solutions:
            - Find places you can go from home (Store A, Store B, Intersection)
            - From each of those places, find all paths you can take from that place
            - Keep track of the distance you've traveled as you go
            - Repeat this process until you get to school
            - Compare the distance you've traveled for each path
            - Find the shortest path

    Basically have a problem you want to solve, then you have systematic instructions for solving the problem.

    Depending on what data structure you are using to store the data, the algorithm might look different. You may have completely different algorithms for solving the same problem depending on what data structure you are using.
        - For this specific example, the hash table would make it easier to write an algorithm because you have all the places you can go from home in one group. Compared to the List data structure where you'd have to go through the entire list.

    Another Example : You're hosting a party, each person that comes to the party is bringing a small ball with thier name written on it. (David will have a ball with "David" written on it.) To keep track of who came to the party in order. To come up with a system to store the balls to keep track of who came to the party........

        Solution 1: Very long box with 100 partitions, all have same size and shape. Everytime someone comes to the party you put the ball in a slot in the order they came to the party. === This is an Array data structure...

        Solution 2: Instead of a long box with many partitions you get individual boxes that are connected with strings (1st => 2nd; 2nd => 3rd; 3rd => 4th;). Continue to put balls in the order they come in. === This is the linked list data structure...

    Problem 1 :
        100 people show up to the party, 98th person mispelled their name. To fix the array data structure is easy because you just need to find the 98th partition which is easy to calculate since each patition is 10cm wide(10cm * 97) would give you the 98th partition. Then replace with correct token.

        The same problem with the linked list data structure is tricky because you need to find the 98th box which is harder. The strings can be any length so each box can be in any location relative to the previous box. To find the 98th box you'd need to count them one by one.

    Problem 2: 100 people show up to the party but 5 people show up unexpected.

        With linked list data structure it is easy to deal with because you only need to add 5 more boxes to the linked list.

        With array data structure it is trickier. One option is to get another box with 100 partitions store them there and use the two boxes together. Or you can destroy the boxes you had and get a box with more partitions like 200 and transfer all the balls you had to the new box. Then add the addition 5 peoples tokens. If you have no idea how many people are coming to the party the linked list data structure will be easier than the array data structure.

    This is a roughly simple idea to think about Data Structures...
