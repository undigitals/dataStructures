# Hash table structures

### All structure and functions are in the **hash_table** header file.

we will create a ** hash_item ```struct``` ** to store ** value ** and ** key ** of the each item.

``` C 

typedef struct hash_item{
    int* val;
    int* key;
}hash_item;

```
Now we need a ** hash_table ```struct``` ** to store all the items structure (to store all ``` hash_item ```) using array of pointers, and in this structure we need: 
* ``` int size  // size of table ``` 
* ``` int count // how full the table ```

```C
typedef struct hash_table{
    int size;
    int count;
    hash_item** items;
}hash_table;

```