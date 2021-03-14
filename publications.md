---
layout: page
title: Publications
---

<p class="message">
  Hey there! This page is included as an example. Feel free to customize it for your own use upon downloading. Carry on!
</p>

In the novel, *The Strange Case of Dr. Jeykll and Mr. Hyde*, Mr. Poole is Dr. Jekyll's virtuous and loyal butler. Similarly, Poole is an upstanding and effective butler that helps you build Jekyll themes. It's made by [@mdo](https://twitter.com/mdo).

There are currently two themes built on Poole:

* [Hyde](https://hyde.getpoole.com)
* [Lanyon](https://lanyon.getpoole.com)

Learn more and contribute on [GitHub](https://github.com/poole).

<!-- High Dimensional Statistics -->
<h3  class="pubyear">High Dimensional Statistics</h3>
{% bibliography -f hds %}

<!-- Social Network Analysis --> 
<h3  class="pubyear">Social Network Analysis</h3>
{% bibliography -f sna %}

{% for y in page.years %}
  <h3  id="{{y}}" class="pubyear">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}


