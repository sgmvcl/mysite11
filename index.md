@def title = "Michael using Franklin"
@def hasmath = true
@def hascode = true

# Set up
### update title
### update config.md file

* change author

* add site name for GitHub

### create a table of contents 
\toc

### upload using GitHub desktop

# Examples
### how to enter text
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse finibus suscipit augue sed euismod. Proin laoreet convallis nisi, sed aliquet mi tincidunt sit amet. Vivamus maximus augue nec est pretium cursus vitae sed mi. Aenean vestibulum malesuada mattis. Phasellus metus neque, varius quis tincidunt porttitor, bibendum vel enim. Curabitur vitae imperdiet sapien, ut pretium ante. Suspendisse quam nisi, tristique vel tincidunt non, accumsan et libero. In varius enim sit amet vulputate vulputate. Suspendisse sed quam vitae lacus suscipit imperdiet vehicula sit amet est. Mauris nisl ipsum, auctor non odio nec, maximus tempor ex.

### how to render math equations

$$ \bar{x} = \frac{1}{n} \Bigg(\sum_{i=1}^{n} x_i \Bigg) = \frac{x_1 + x_2 + \cdots + x_n}{n} $$ #

$$ s = \sqrt{\frac{1}{N-1} \sum_{i=1}^{N} (x_i - \bar{x})^2} $$ #

$$
    M = 
        \begin{bmatrix}
            \begin{aligned}
                &2 & &1 & -&1 \space \\
                \space -&3 & -&1 & &2 \\
                -&2 & &1 & &2
            \end{aligned}
        \end{bmatrix}
$$

### how to insert Julia code with outputs
Hello world!

```julia:./ex15
println("Hello world!")
```

\show{./ex15}

Basic Math

```julia:./ex56
4^3
```
\show{./ex56}

Create Function

```julia:./ex17
function add(x, y)
    x + y
end
```

\show{./ex17}

Call Function

```julia:./ex20
add(2, 7)
```

\show{./ex20}

Random Numbers

```julia:./ex15
rand(5, 5)
```

\show{./ex15}

### how to insert a table from csv file
World´s population:
\tableinput{}{./tableinput/exampletable.csv}

@@source
Source: Wiki
@@

### how to insert an image file
![GDP to debt ratio](/assets/GDP_to_debt_ratio.png)

### how to insert a clickable thumbnail to a youtube video
[![YT](https://img.youtube.com/vi/ey7DqMbkxj4/0.jpg)](https://youtu.be/ey7DqMbkxj4)

### how to inject raw HTML

~~~
<iframe width="1080" height="720" src="https://www.youtube.com/embed/ey7DqMbkxj4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
~~~


<!-- Earthquakes stronger than mag 6 since 2000:
\tableinput{}{./tableinput/query_USGS.csv}

@@source
Source: USGS
@@ -->

<!-- # Franklin syntax sandbox

This page is meant as a sandbox for Franklin Syntax so that you can quickly practice or experience things.

## Sandbox

Write whatever you want here to practice Franklin Syntax:

```julia:./ex1
using LinearAlgebra, Random
Random.seed!(135)
a, b = randn(50), randn(50)
println(dot(a, b))
println(sum(ai * bi for (ai, bi) ∈ zip(a, b)))
```

\output{./ex1}

(yet another example that floating point arithmetics can be complicated).

$$ \forall x \in \R:\quad \scal{x, x} \ge 0 $$

\newcommand{\E}{\mathbb E}

Surely some people remember the ordering, but I always forget:

$$ \varphi(\E[X]) \le \E[\varphi(X)] $$

for $\varphi$ convex. -->
