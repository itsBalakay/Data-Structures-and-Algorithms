Data Structures & Algorithms #2 - An Overview of Arrays and Memory (CS Dojo)

Array === Collection of items of a single type :
[5, -2, 300, 20] = arr of integers
["yeahhh", "ouch", "haha"] = arr of strings
["ahhh", 3, 2, 1, "ohh"] !== very unusual for arr to have multiple types of values

    There are two mechanisms for storing data on your computer:
        1 : Memory (RAM)
        2 : Storage (HDD, SSD)

        difference is the data on storage is permanently stored while the data on memory is not.

        For example : When you are working on essay and your computer crashes if you lose all your work... it was probably being store on the memory. But when you hit the save button it becomes a file within your storage.

        Why wouldnt you just store everything on storage ?
            - reading and writing data into storage is slow... like walking to the file cabinet and getting a file.
            - Memory is like a temporary desk in your room. So when you retrieve the files from storage you can put them on this temporary desk so it will be faster to work on them. It is a lot faster to write data and read data from memory. When you finish working on the memory stored files you can bring them back to the storage so they will be there permanently.(This is how memory and storage work together for files)


        Applications:
            - Applications are normally stored on storage, but when you launch one it loads onto the memory so its faster to use and access. So if you run too many apps at the same time you might run out of memory. This is why your computer slows down if you run too many sometimes.

    How is this related to programming ?.... Particulary Arrays ?

        ex: int a = 1; --- this is stored on memory
            each integer when stored on a computer is expressed as 32 ones and zeros.
                int a = 1; is 31 zeros.. and 1 one at the end of it.
                int a = 2; is 30 zeros a one and then another zero

                each zero and one is called a bit (bit = 1 or 0)
                 -> 32 bits for integer

        Memory can be thought of as a long tape of bytes.
            A byte is a small unit of data === 8 bits (ex: 10010101)
            each byte in memory is given an address represented by an integer.
            the operating system determines the address of the application you open.

        How can you store an integer on memory?
            - take four bytes and use that to represent an integer (4 bytes * 8(8 bits = 1 byte) === 32) 32 bits for an integer.
                this is what a computer does.

            int 1 converted into 32 bits... those bits are split into 4 bytes.. then stored in those bytes. If you have int b = 3; on the next line that integer would be stored on the next 4 bytes in the memory.

        Idea is the same for decimals and characters altough you might need different number of bytes.

        If you wanted to store an array of integers.... the number of bytes needed is dependent on the amount of data. 3 integers in array === 12 bytes
