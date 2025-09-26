# Ex-3(C) Expression Tree
## AIM:
To write a C function to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.

## Algorithm
1. Start 
2. Print node data in preorder then traverse left then right 
3. Traverse left in inorder then print node data then traverse right 
4. Traverse left in postorder then traverse right then print node data 
5. Recursive approach is used for all three traversal methods 
6. Functions handle each tree node using tree->d, tree->l, tree->r 
7. End 
## Program:
```
/*
Program to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.
Developed by: ARSHATHA
RegisterNumber:  212222230012
*/
/*
struct n { char d; struct n*l; struct n*r;
};*/
voidpreOrder(struct n*tree)
{
if(tree)
{
printf("%c",tree->d); preOrder(tree->l); preOrder(tree->r);
}
}
void inOrder(struct n*tree)
{
if(tree)
{
inOrder(tree->l); printf("%c",tree->d); inOrder(tree->r);
}
}
voidpostOrder(struct n*tree)
 
{
if(tree)
{
postOrder(tree->l); postOrder(tree->r); printf("%c",tree->d);
}
}


```

## Output:

![image](https://github.com/user-attachments/assets/6faa9c9b-d780-4a03-8ff8-14ea2a57e39d)



## Result:
Thus, the C program to display the Expression Tree in the format of In-order ,Pre-order and Post-order traversal.
