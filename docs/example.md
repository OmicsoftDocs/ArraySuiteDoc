title: my examples
description: examples of using mkdoc extensions, balah, bapla
path: https://github.com/welcomege/welcomege.github.io/blob/master/doc/attachments/test1.txt
source: test1.txt

## First

For full documentation visit [mkdocs.org](http://mkdocs.org).

### Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs help` - Print this help message.

### Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

## Images, videos and table

### Simple image
![logo](images/logo.png)

Test a large image

![logo](images/test1.png)

### lightbox image
Test large image with lightbox using extend theme_dir

<a href="https://unsplash.it/1200/768.jpg?image=250" data-toggle="lightbox" data-title="A random title" data-footer="A custom footer text">
    <img src="https://unsplash.it/300.jpg?image=250" class="img-fluid">
</a>

### lightbox gallery

<div class="row">
    <div class="offset-md-2 col-md-8">
        <div class="row">
            <a href="https://unsplash.it/1200/768.jpg?image=251" data-toggle="lightbox" data-gallery="example-gallery" class="col-sm-4">
                <img src="https://unsplash.it/600.jpg?image=251" class="img-fluid">
            </a>
            <a href="https://unsplash.it/1200/768.jpg?image=252" data-toggle="lightbox" data-gallery="example-gallery" class="col-sm-4">
                <img src="https://unsplash.it/600.jpg?image=252" class="img-fluid">
            </a>
            <a href="https://unsplash.it/1200/768.jpg?image=253" data-toggle="lightbox" data-gallery="example-gallery" class="col-sm-4">
                <img src="https://unsplash.it/600.jpg?image=253" class="img-fluid">
            </a>
        </div>
        <div class="row">
            <a href="https://unsplash.it/1200/768.jpg?image=254" data-toggle="lightbox" data-gallery="example-gallery" class="col-sm-4">
                <img src="https://unsplash.it/600.jpg?image=254" class="img-fluid">
            </a>
            <a href="https://unsplash.it/1200/768.jpg?image=255" data-toggle="lightbox" data-gallery="example-gallery" class="col-sm-4">
                <img src="https://unsplash.it/600.jpg?image=255" class="img-fluid">
            </a>
            <a href="https://unsplash.it/1200/768.jpg?image=256" data-toggle="lightbox" data-gallery="example-gallery" class="col-sm-4">
                <img src="https://unsplash.it/600.jpg?image=256" class="img-fluid">
            </a>
        </div>
    </div>
</div>

### lightbox Youtube
<p><a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ" data-toggle="lightbox">Justin Bieber - Love Yourself</a></p>

### TestTable
| Header One     | Header Two     | Header One     | Header Two     |
| :------------- | :------------- | :------------- | :------------- |
| Item One       | Item Two       | Item One       | Item Two       |

## Extensions
###  Admonition

use below

``` markdown
!!! note
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
```

will have:

!!! note
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

!!! tip
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
    more to find in [squidfunk](http://squidfunk.github.io/mkdocs-material/extensions/admonition/)


!!! Summary "Open styled details"
    !!! danger "Nested details!"
        And more content again.

!!! tip "Tip: we can add code here"
    ``` python hl_lines="3 4"
    """ Bubble sort """
    def bubble_sort(items):
        for i in range(len(items)):
            for j in range(len(items) - 1 - i):
                if items[j] > items[j + 1]:
                    items[j], items[j + 1] = items[j + 1], items[j]
    ```

!!! seealso
    Ref1:
    Ref2:

!!! summary
    Summary style

!!! done
    I am done

!!! warning
    my warning

!!! failure
    A fail case

!!! danger
    be careful

!!! bug
    It is a bug

!!! quote
    someone said so.

[More details](http://squidfunk.github.io/mkdocs-material/extensions/admonition/)

### Details

???+ note "Open styled details"

    ??? danger "Nested details!"
        And more content again.

styled details

!!! note
    ???+ "Open styled details"
        Hello1
        Hello2
    !!! danger
        ??? "Nested details!"
            And more content again.


### Footnotes
Example:

``` markdown
Lorem ipsum[^1] dolor sit amet, consectetur adipiscing elit.[^2]
```

Result:

Lorem ipsum[^1] dolor sit amet, consectetur adipiscing elit.[^2]

[^1]: Lorem ipsum dolor sit amet, consectetur adipiscing elit.
[^2]:
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

### Code highlight
``` python
import tensorflow as tf
```

Code highlight the 3rd and 4th lines

``` python hl_lines="3 4"
""" Bubble sort """
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

[More examples of code highlight](https://github.com/squidfunk/mkdocs-material/blob/master/docs/extensions/codehilite.md)

### smart symbols
- (tm)
- (r)
- [more](https://facelessuser.github.io/pymdown-extensions/extensions/smartsymbols/)

### meta
See the meta and description above.

### Task list
Task List

- [X] item 1
    * [X] item A
    * [ ] item B
        more text
        + [x] item a
        + [ ] item b
        + [x] item c
    * [X] item C
- [ ] item 2
- [ ] item 3

### emoji
EmojiOne :smile: emoji are very useful :thumbsup:.

You can also escape `:` characters to escape the emoji: \:smile:.

### Super and sub using caret and tilde, and mark

- ^^underline me^^
- H^2^0
- text^a\ superscript^
- ~~delete me~~
- CH~3~CH~2~OH
- text~a\ subscript~
- ==mark me==
- ==mark== ==me==

### Keyboard using keys

To copy, press ++ctrl+alt+c++ for Windows or Linux or ++cmd+alt+c++ for Mac.

You can also use custom key labels: ++ctrl+alt+"&Uuml;"++.

### Mathjax
Some Block Equations:

$$
\frac{n!}{k!(n-k)!} = \binom{n}{k}
$$

$$
#E(\mathbf{v}, \mathbf{h}) = -\sum_{i,j}w_{ij}v_i h_j - \sum_i b_i v_i - \sum_j c_j h_j
$$

\[3 < 4\]

\begin{align}
    p(v_i=1|\mathbf{h}) & = \sigma\left(\sum_j w_{ij}h_j + b_i\right) \\
    p(h_j=1|\mathbf{v}) & = \sigma\left(\sum_i w_{ij}v_i + c_j\right)
\end{align}

Inline equations: $p(x|y) = \frac{p(y|x)p(x)}{p(y)}$, \(p(x|y) = \frac{p(y|x)p(x)}{p(y)}\).

## Reference
http://squidfunk.github.io/mkdocs-material/extensions/pymdown/
