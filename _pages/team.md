---
title: "HBML - Team"
layout: gridlay
excerpt: "HBML: Team members"
sitemap: false
permalink: /team/
---
<head>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">
</head>

<style>
h4 {
    margin-bottom: 4px; /* Adjust this value as needed */
  }

.member-info {
  margin: 0;
}

.contact-icons {
  display: flex;
  align-items: center;
  margin-top: 5px;
}
.contact-icons a {
  margin-right: 10px;
  text-decoration: none;
  color: inherit;
}
.contact-icons i {
  font-size: 1.2em;
}

.well {
  height: 300px; /* Adjust the height as needed */
  overflow: auto; /* Add scroll if content exceeds the height */

  .clearfix::after {
  content: "";
  display: table;
  clear: both;
}
}
</style>

# Group Members
<div>
{% assign number_printed = 0 %}
{% for member in site.data.hbml_team %}

{% assign even_odd = number_printed | mod: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/team/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />

  <!--If lab member has their own website, insert it-->
  {% if member.website %}
  <h4>[{{ member.name }}]({{member.website}})</h4>
  {% else %}
  <h4>{{ member.name }}</h4>
  {% endif %}


  <p class="member-info"><strong>Role:</strong> {{ member.info }}</p> 
  {% if member.background %}
  <p class="member-info"><strong>Background:</strong> {{ member.background }}</p>
  {% endif %}

<div class="contact-icons">
  {% if member.email %}
  <a href="mailto:{{ member.email }}" title="Email">
    <i class="fas fa-envelope"></i>
  </a>
  {% endif %}
  {% if member.linkedin %}
  <a href="{{ member.linkedin }}" title="LinkedIn" target="_blank">
    <i class="fab fa-linkedin"></i>
  </a>
  {% endif %}
  {% if member.x %}
  <a href="{{ member.x }}" title="X (Twitter)" target="_blank">
    <i class="fab fa-twitter"></i>
  </a>
  {% endif %}
 {% if member.bluesky %}
  <a href="{{ member.bluesky }}" title="Bluesky" target="_blank">
    <i class="fa-brands fa-bluesky"></i>
  </a>
  {% endif %}
  {% if member.github %}
  <a href="{{ member.github }}" title="Github" target="_blank">
    <i class="fab fa-github"></i>
  </a>
  {% endif %}
</div>

</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | mod: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}
</div>

<div class="clearfix"></div>

<hr> <!-- Add a horizontal rule here -->

## Alumni
{% for member in site.data.alumni_members %}
{% if member.website %}
  <p><b>[{{ member.name }}]({{member.website}})</b>
  {% else %}
  <p><b>{{ member.name }}</b>
  {% endif %}
  Role in the lab: {{ member.role_then }} <br>
  After: {{ member.role_after }} <br></p>
 {% endfor %}

<hr> <!-- Add a horizontal rule here -->

## Collaborators
{% for collab in site.data.collaborators %}
  <b>{{ collab.name }}</b> - <i>{{ collab.institute }}</i>
{% endfor %}

<hr> <!-- Add a horizontal rule here -->

## Administrative Support
We have help. But we won't tell you our sources.