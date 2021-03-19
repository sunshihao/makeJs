js 解释器 20210319 晴 
# makeJs

For leaning how to do a interpreter. 

So I make a sub Javascript interpreter for interpreting itself.
(No dependence any third-party)


# In developing

Now support：

* define variables
* simple expression
* compares
* if statement
* while loop
* Function
* Array


![demo.jpg](/demo.gif)

```js

function quickSort(list,len) {
    let a = 0;
    let b = len-1;
    let c = list[a];
    while (a < b){
        while (list[b]>c && a < b){
            b = b-1;
        }
        if(list[b] < c){
            list[a] = list[b];
            list[b] = c;
            b = b-1;
            c = list[b];
        }
         while (list[a] < c && a < b){
            a = a + 1;
         }
        if(list[a] > c){
            list[b] = list[a];
            list[a] = c;
            a = a + 1;
            c = list[a];
        }
    }
    return list;
}

let arr = [9,3,2,1,5,-2,6];
quickSort(arr,7);

```

See <a href="https://github.com/zuluoaaa/makeJs/tree/master/test">the test folder</a> for more examples
 
 # Future support:
 * Object
 * ...
 
 
 
