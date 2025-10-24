# CYB-2013 Project 02 — Website Traversal
## Objective

The goal of this project was to develop a web crawler and link traversal program in Python to explore internal hyperlinks on a website.  
The assignment reinforced understanding of graph traversal algorithms (BFS and DFS) and pathfinding in a real-world web context.

The program uses the BeautifulSoup 4 library to parse HTML and extract `<a>` tags, building a graph that maps each page to its outbound links.

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

Example:
```python
G['/index.html'] = ['alink.html', 'blink.html', 'clink.html', 'index.html']
