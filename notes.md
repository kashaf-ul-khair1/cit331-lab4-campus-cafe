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

## Specificity experiment
The #main p selector is stronger than .hero p, so the paragraph becomes red. When I change #main p to main p, the paragraph becomes white because .hero p is stronger.

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

## Bug log (Lab 4, Task 6)

| # | What was wrong | Which tool showed it | My fix |
|---|---|---|---|
| 1 | HTML linked to `style.css`, but the file was named `bugs.css`. | Network | Changed the link to `bugs.css`. |
| 2 | HTML had no language attribute. | W3C Validator | Added `lang="en"`. |
| 3 | Image had no alt attribute. | W3C Validator | Added `alt="Campus Cafe logo"`. |
| 4 | Label's `for` value did not match the input ID. | W3C Validator | Changed `for="mail"` to `for="email"`. |
| 5 | Heading jumped from h1 to h4. | W3C Validator | Changed h4 to h2. |
| 6 | Menu links were not inside a navigation landmark. | Accessibility inspection | Replaced the menu div with nav. |
| 7 | CSS property `colour` was misspelled. | CSS inspection | Changed `colour` to `color`. |
| 8 | Semicolon was missing after the button hover background. | CSS inspection | Added the semicolon. |
| 9 | CSS selector `.notes` did not match HTML class `.note`. | CSS inspection | Changed `.notes` to `.note`. |
| 10 | Note text had low contrast. | Accessibility improvement | Changed `#999999` to `#555555`. |


## Live site observations (Lab 4, Task 7)

### 1. Localhost vs Live Site
My local website uses HTTP, but my live website uses HTTPS. The server and remote address are different because localhost runs on my computer while the live website runs on gitHub Pages.

### 2. HTTPS and Security
The padlock shows that the connection is secure and the certificate is valid. If the website used HTTP someone on the same Wi-Fi could read or change the data sent between the user and the website.

### 3. Local Storage
The saved orders table was empty on the live website because localhost and the live website save data separately. Orders saved on my computer do not appear automatically on the live website.

### 4. Missing Page
The missing page showed error 404, which means the page was not found. The response came from the website's server.