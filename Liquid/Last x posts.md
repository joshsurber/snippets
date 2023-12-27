
``` liquid
{% assign top_posts = collections.posts | reverse %}  
{%- for post in top_posts limit:5 -%}  
<!-- post content -->  
{%- endfor -%}
```