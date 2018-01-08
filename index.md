---
layout: page
title: Ram K Mazumder
subtitle: PhD Candidate, Case Western Reserve University
meta-title: "Hi, I'm RK"
use-site-title: true
bigimg:
  - /img/rkk1.jpg: Case Western Reserve Uni Campus
  - /img/hnw.jpg: Happy New Year 2018
---

<!-- Typed.js --> 
<script src="/js/jquery-1.11.2.min.js"></script>
<script src="/js/typed.js" type="text/javascript"></script>
<script>
  $(function(){
    $(".typed").typed({
      strings: ["Technology.","Open Source.","Mathematics.","Space and Universe.","Science.","Art.","Ubuntu."],
      typeSpeed: 100,
      loop: true,
      backDelay: 1000
    });
  });
</script>

<div class="typed-js-hide">
  <div class="row">
    <div class="col-sm-12">
      <div class="text-center">
          <h1>I write about <span class="typed" style="color:#a50509";></span></h1>
      </div>
    </div>
  </div>
</div>

<!-- site body (untouched)--> 
<div class="posts-list">
  {% for post in paginator.posts %}
  <article class="post-preview">
    <a href="{{ post.url | prepend: site.baseurl }}">
    <h2 class="post-title">{{ post.title }}</h2>

    {% if post.subtitle %}
    <h3 class="post-subtitle">
      {{ post.subtitle }}
    </h3>
    {% endif %}
    </a>

    <p class="post-meta">
      Posted on {{ post.date | date: "%B %-d, %Y" }}
    </p>

    <div class="post-entry-container">
      {% if post.image %}
      <div class="post-image">
        <a href="{{ post.url | prepend: site.baseurl }}">
          <img src="{{ post.image }}">
        </a>
      </div>
      {% endif %}
      <div class="post-entry">
        {{ post.excerpt | strip_html | xml_escape | truncatewords: site.excerpt_length }}
        {% assign excerpt_word_count = post.excerpt | number_of_words %}
        {% if post.content != post.excerpt or excerpt_word_count > site.excerpt_length %}
          <a href="{{ post.url | prepend: site.baseurl }}" class="post-read-more">[Read&nbsp;More]</a>
        {% endif %}
      </div>
    </div>

    {% if post.tags.size > 0 %}
    <div class="blog-tags">
      Tags:
      {% if site.link-tags %}
      {% for tag in post.tags %}
      <a href="{{ site.baseurl }}/tag/{{ tag }}">{{ tag }}</a>
      {% endfor %}
      {% else %}
        {{ post.tags | join: ", " }}
      {% endif %}
    </div>
    {% endif %}

   </article>
  {% endfor %}
</div>

{% if paginator.total_pages > 1 %}
<ul class="pager main-pager">
  {% if paginator.previous_page %}
  <li class="previous">
    <a href="{{ paginator.previous_page_path | prepend: site.baseurl | replace: '//', '/' }}">&larr; Newer Posts</a>
  </li>
  {% endif %}
  {% if paginator.next_page %}
  <li class="next">
    <a href="{{ paginator.next_page_path | prepend: site.baseurl | replace: '//', '/' }}">Older Posts &rarr;</a>
  </li>
  {% endif %}
</ul>
{% endif %}


## Other Affiliation
Assistant Professor (on leave),
Institute of Earthquake Engineering Research,
Chittagong University of Engineering and Technology,
Chittagong 4349, Bangladesh

President, South Asian Chapter, Erasmus Mundus Students and Alumni Association


## Tweets
<p>
 <a class="twitter-timeline"
 href="https://twitter.com/rkmazumder"
 data-chrome="nofooter noborders transparent" data-tweet-limit="3">I am tweeting (@rkmazumder)</a>
 <script>
						!function(d, s, id) {
							var js, fjs = d.getElementsByTagName(s)[0], p = /^http:/
									.test(d.location) ? 'http' : 'https';
							if (!d.getElementById(id)) {
								js = d.createElement(s);
								js.id = id;
								js.src = p
										+ "://platform.twitter.com/widgets.js";
								fjs.parentNode.insertBefore(js, fjs);
							}
						}(document, "script", "twitter-wjs");
 </script>
</p>

## Erasmus Scholarship
<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vTEwZvTVZI9SWr7IHNNgtqyVvNcZWLudMI278jvWaPcl67O_eZQzJ4vPHVugiQ1nwWytmZeoPXAVo2T/embed?start=false&loop=false&delayms=5000" frameborder="0" width="512" height="400" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

### Blog Post
<div class="posts-list">
  {% for post in paginator.posts %}
  <article class="post-preview">
    <a href="{{ post.url | prepend: site.baseurl }}">
	  <h2 class="post-title">{{ post.title }}</h2>

	  {% if post.subtitle %}
	  <h3 class="post-subtitle">
	    {{ post.subtitle }}
	  </h3>
	  {% endif %}
    </a>

    <p class="post-meta">
      Posted on {{ post.date | date: "%B %-d, %Y" }}
    </p>

    <div class="post-entry-container">
      {% if post.image %}
      <div class="post-image">
        <a href="{{ post.url | prepend: site.baseurl }}">
          <img src="{{ post.image }}">
        </a>
      </div>
      {% endif %}
      <div class="post-entry">
        {{ post.excerpt | strip_html | xml_escape | truncatewords: site.excerpt_length }}
        {% assign excerpt_word_count = post.excerpt | number_of_words %}
        {% if post.content != post.excerpt or excerpt_word_count > site.excerpt_length %}
          <a href="{{ post.url | prepend: site.baseurl }}" class="post-read-more">[Read&nbsp;More]</a>
        {% endif %}
      </div>
    </div>

    {% if post.tags.size > 0 %}
    <div class="blog-tags">
      Tags:
      {% if site.link-tags %}
      {% for tag in post.tags %}
      <a href="{{ site.baseurl }}/tag/{{ tag }}">{{ tag }}</a>
      {% endfor %}
      {% else %}
        {{ post.tags | join: ", " }}
      {% endif %}
    </div>
    {% endif %}

   </article>
  {% endfor %}
</div>

{% if paginator.total_pages > 1 %}
<ul class="pager main-pager">
  {% if paginator.previous_page %}
  <li class="previous">
    <a href="{{ paginator.previous_page_path | prepend: site.baseurl | replace: '//', '/' }}">&larr; Newer Posts</a>
  </li>
  {% endif %}
  {% if paginator.next_page %}
  <li class="next">
    <a href="{{ paginator.next_page_path | prepend: site.baseurl | replace: '//', '/' }}">Older Posts &rarr;</a>
  </li>
  {% endif %}
</ul>
{% endif %}



## Contact

```
Department of Civil Engineering
Case Western Reserve University
Cleveland, OH 44106

Office: Bingham 277
Email: rkmazumder[at]gmail.com
```
