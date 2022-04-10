## Welcome to DataStructure Blogs 

We will be learning about data structures in this blog.Data Strucure can be learnt using any basic programming language and for this blog we will be using JAVA.Our focus will be on basic construction using JAVA and then on the usage of the data strcuture. The examples using the code will emphasize on the real life use cases of the data structures.


You can use the [editor on GitHub](https://github.com/piyushutreja/DataStructureBolgs/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

## Types of Data Structures
### 1.Linear Data Structure
### 2.Non Linear Data Structre


#### Linked List

The linked list has following fucntions 
1.Insertion:- 
  -Insertion at end.
  -Insertin at a specific place.
2.Traversal
3.Deletion
4.Search


##### Construction of Basic Linked List 

```
public  class LinkedList {

     public static void main(String []args){
        System.out.println("Hello World");
    
    LinkedList list = new LinkedList();
    
    list = list.insert(list,1);
    list = list.insert(list,2);
    list = list.insert(list,3);
    list = list.insert(list,4);
    list = list.insert(list,5);
    
    printList(list);
    
     }



    
    Node head; 
    
 static   class Node {
        
        int data; 
        Node next; 
        
        Node(int d) 
        {
            data = d;
        }
    }


//Insertion Data
//1.If linked list is empty it new node will become head
//2.If the element is already there the node will be added to end and it will poin to null


public static LinkedList insert(LinkedList list,int data)
{
 //Create Node with data
 Node new_node = new Node(data);
 new_node.next = null; 
 //
 if(list.head == null)
 {
     list.head = new_node; 
  }
 
  else
  {
      
      //Traverse to last Node and insert node there
      
      Node last = list.head; 
      while (last.next != null)
      {
          last = last.next;
      }
      
      last.next = new_node;
  }
    return list; 
}

public static void printList(LinkedList list )
{
    Node currNode = list.head; 
    
    while (currNode.next != null)
    {
        System.out.println(currNode.data);
        
        currNode = currNode.next;
    }
}

}

```



```tst

dfjfsd sd

```


Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/piyushutreja/DataStructureBolgs/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
