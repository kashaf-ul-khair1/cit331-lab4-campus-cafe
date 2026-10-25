# HTTP Observations (Lab 4, Task 1)

| Question | My Answer |
|---|---|
| Request method for index.html | GET |
| Status code with Disable cache ticked | 200 |
| Status code on a normal reload | 200 |
| Status code for /nothing-here.html | 404 |
| Value of Content-Type response header | text/html |
| Remote Address (IP and port) | 127.0.0.1:5500 |
| Protocol in the address bar | http |

## Why is this address HTTP and not HTTPS?

This website uses HTTP because I am running it on my computer using Live Server. HTTPS protects data sent over a network while my local website is running on my own computer.

## Selectors I used

| Selector kind | Example from my CSS |
|---|---|
| Element | `body` |
| Class | `.hero` |
| ID | `#main` |
| Grouping (comma) | `h1, h2, h3` |
| Descendant (space) | `.nav-list a` |
| Child (`>`) | `main > section` |
| Adjacent sibling (`+`) | `h1 + p` |
| Compound (no space) | `a.active` |
| Attribute | `a[href^="http"]` |
| Pseudo-class | `a:hover` |
| Pseudo-element | `.menu-group h2::before` |

## Specificity experiment
The #main p selector is stronger than .hero p, so the paragraph becomes red. When I change #main p to main p, the paragraph becomes white because .hero p is stronger.