---
layout: page
title: About 
<!--tagline: Supporting tagline-->
---
{% include JB/setup %}

These are the collaboratively-constructed class notes for UCSD's CSE 202: Graduate Algorithms, taught in winter 2014 by [Russell Impagliazzo](http://cseweb.ucsd.edu/~russell/). 
The idea is that the students together can create a better resource than any one person.

###Links

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



To contribute, [fork this project on GitHub](https://github.com/emchristiansen/CSE202) and send me a pull request.

Read [Jekyll Quick Start](http://jekyllbootstrap.com/usage/jekyll-quick-start.html)

Complete usage and documentation available at: [Jekyll Bootstrap](http://jekyllbootstrap.com)
