---
layout: page
title: About 
<!--tagline: Supporting tagline-->
---
{% include JB/setup %}

<a href="https://github.com/emchristiansen/CSE202">
  <img style="position: absolute; top: 0; right: 0; border: 0;" src="https://s3.amazonaws.com/github/ribbons/forkme_right_darkblue_121621.png" alt="Fork me on GitHub">
</a>

<script type="text/x-mathjax-config">
MathJax.Hub.Config({
  tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}
});
</script>

<script type="text/javascript"
  src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>

These are the collaboratively-constructed class notes for UCSD's CSE 202: Graduate Algorithms, taught in winter 2014 by [Russell Impagliazzo](http://cseweb.ucsd.edu/~russell/). 
The idea is that the students together can create a better resource than any one person.

##Links

The class webpage is [here](http://cseweb.ucsd.edu/classes/wi14/cse202-a/).

The Piazza page is [here](piazza.com/ucsd/winter2014/cse202/home).

There's a [previous set of notes](http://cseweb.ucsd.edu/~ncjones/cse202/), compiled in the fall of 2002 by Neil Jones.
These are another great resource, as the curriculum hasn't changed too much in the last decade.

#Notes

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

#Contributing

We strongly encourage / need students to contribute notes.
These contributions can be as large as the entire notes for one day, or as small as a fixed typo.

To contribute, [fork this project on GitHub](https://github.com/emchristiansen/CSE202) and send me a pull request.
You'll find notes for each day in the `_posts` folder.

You should be able to see your changes by pushing your own GitHub branch and going to `http://<username>.github.io/CSE202`.
GitHub will run Jekyll to process the markdown, etc, and generate the site.

For more information on GitHub's publishing tools, see [here](http://pages.github.com/).
For more on Jekyll, see the [Jekyll Quick Start](http://jekyllbootstrap.com/usage/jekyll-quick-start.html).
For info on Jekyll Bootstrap, which was used to generate this site, see [here](http://jekyllbootstrap.com).

##Math markup

We're using [MathJax](http://www.mathjax.org/) to get $\LaTeX$-style math in the browser.
This is more fun than generating a boring old PDF, right?

You render inline $\LaTeX$ using the dollar sign (`$`) and block $\LaTeX$ using double dollar signs (`$$`).
For example, the probability of getting $k$ heads when flipping $n$ coins is $P(E) = {n \choose k} p^k (1-p)^{ n-k}$.
And here are the Lorenz Equations:
$$  
\begin{aligned}
\dot{x} &= \sigma(y-x) \cr
\dot{y} &= \rho x - y - xz \cr
\dot{z} &= -\beta z + xy
\end{aligned}
$$

