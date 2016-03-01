---
layout: post
date: 2016-03-01 12:00:00 -0800
title: "Sample Blog Post"
comments: true
categories: [showcase, static blogging, jekyll]
---
I generated this prestyled page by running command: `$ rake new_post["Sample Blog Post"]`

I write content that looks like this:
<hr>
<div> 
# Heading<br />
 - Item 1<br />
 - Item 2<br />
 - Item 3<br />
<br />
 *sample code snippet*<br />
<br />
</div>

{% assign openTag = '{' %}
{{ openTag }}% codeblock hello_world.rb %}<br />
def hello_world<br />
&nbsp;&nbsp;puts "Hello world"<br />
end<br />
{{ openTag }}% endcodeblock %}<br />


**Output:**
<hr>

# Heading
 - Item 1
 - Item 2
 - Item 3

*sample code snippet*

{% codeblock hello_world.rb %}
def hello_world
  puts "Hello world"
end
{% endcodeblock %}
