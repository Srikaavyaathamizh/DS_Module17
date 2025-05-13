# Ex21 Representation of Graph
## DATE:04/5/2025
## AIM:
To write a C program to display the adjacency matrix of the given graph by supplying the edges and the number of vertices.

## Algorithm
1.Start and read number of vertices V. 2.Declare and initialize adjMatrix[V][V] to 0. 3.Compute max edges me = V * (V - 1) / 2. 4.For each edge, read e1 and e2; add to matrix until e1 == -1 && e2 == -1. 5.Print the adjacency matrix and end.
## Program:
```
/*
Program to display the adjacency matrix of the given graph
Developed by: SRIKAAVYAA T
RegisterNumber:  212223230214
*/
#include<stdio.h>
int V;
//init matrix to 0
void init(int arr[][V])
{
int i,j;
for(i = 0; i < V; i++)
for(j=0;j<V;j++)
arr[i][j] =0;
}
*/
int main()
{ int e1,e2,me,n,i;
scanf("%d",&V);
int adjMatrix[V][V];
init(adjMatrix);
n=V;
me=n*(n-1)/2;
for(i=0;i<me;i++)
{
scanf("%d%d",&e1,&e2);
addEdge(adjMatrix,e1,e2);
if(e1==-1 &&e2==-1)
{
break;
}
}
printAdjMatrix(adjMatrix);
}

```

## Output:
![image](https://github.com/user-attachments/assets/fca64a7d-8cba-43a9-b150-ed2594e1f094)



## Result:
Thus, the C program to print the adjacency matrix of the given graph is implemented successfully.
