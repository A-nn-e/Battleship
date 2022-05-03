# BATTLESHIP: FIRST-FIT HEURISTIC 

First-fit (FF) is an algorithm for bin packing. Its input is a list of items of different sizes. Its output is a packing - a partition of the items into bins of fixed capacity, such that the sum of sizes of items in each bin is at most the capacity. Ideally, we would like to use as few bins as possible. 

The first-fit algorithm uses the following heuristics:

* It keeps a list of open bins, which is initially empty.
* When an item arrives, find the first bin into which the item can fit, if any.
* If such a bin is found, the new item is placed inside it.
* Otherwise, a new bin is opened and the coming item is placed inside it.

The First-fit algorithm works well for smaller boards of sizes 4x4 and 5x5.

![correct](https://user-images.githubusercontent.com/78024291/166553182-91e357e2-c1f8-4e7d-97c0-dcfe388eb862.PNG)

However, as the size of the board increases the solution becomes incorrect and the variation in the solution also increases with the size of the board.

![big board](https://user-images.githubusercontent.com/78024291/166553515-d8ffbdad-53f7-45db-8bcb-2046d5982e47.PNG)

Also, variation in solution can also be seen in the smaller boards though, less frequently.

![correct 2](https://user-images.githubusercontent.com/78024291/166553837-00c3748b-32bd-4a7a-90fe-64818442a092.PNG)
![incorrect 2](https://user-images.githubusercontent.com/78024291/166553850-84ece00c-2c26-495b-877b-7ece7809247b.PNG)

Both the correct and incorrect solutions can be obtained for the same input. This variation and inaccuracy in solutions becomes more frequent as the size of the board increases.
