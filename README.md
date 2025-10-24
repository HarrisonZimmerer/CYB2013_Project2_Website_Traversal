
# CYB-2013 Project 02 — Website Traversal

## Objective

The goal of this project was to develop a web crawler and link traversal program in Python to explore internal hyperlinks on a website.  
The assignment reinforced understanding of graph traversal algorithms (BFS and DFS) and pathfinding in a real-world web context.

The program uses the BeautifulSoup 4 library to parse HTML and extract `<a>` tags, building a graph that maps each page to its outbound links.

---
## Skills Learned

* Implementing **DFS and BFS** traversal algorithms
* Building and traversing **graphs** of webpage hyperlinks
* Using **BeautifulSoup** to parse and extract HTML data
* Handling URL paths and base references dynamically
* Understanding **shortest path** and **maximum depth** algorithms
* Structuring Python projects with modular design and unit tests
* Writing and debugging automated tests with `pytest`

---

## Tools Used

* Python (3.x)
* BeautifulSoup 4
* urllib
* pytest (unit testing)
* VS Code / GitHub Classroom
* Linux / WSL environment

---

## Project Overview

### Implemented Functions

| Function | Description |
| -------- | ------------ |
| `links_dfs(url)` | Returns all links reachable from a starting URL using **Depth-First Search (DFS)** order. |
| `links_bfs(url)` | Returns all links reachable from a starting URL using **Breadth-First Search (BFS)** order. |
| `find_shortest_path(url1, url2)` | Finds and returns the **shortest link path** between two URLs (or reports if none exists). |
| `find_max_depth(url)` | Determines the URL that is **farthest** from the starting page, returning the full path. |

The crawler stores its traversal as a **dictionary** where keys are page URLs and values are lists of linked pages.

## What I Learned

* How graph traversal concepts apply directly to real-world web crawling
* The difference between BFS and DFS in practice
* How to use Python’s collections and URL libraries effectively
* How to build maintainable, testable Python code for algorithmic assignments

---

## Credits

* Project provided by: *University of Tulsa — CYB-2123: Data Structures & Algorithms used in CYB 2013 Secure Software Development
* Instructor: Dr. Pei
