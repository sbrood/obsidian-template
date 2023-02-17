
up:: [[📚 Bibliography]]
tags:: #source/paper
year:: {{date | format("YYYY")}}
title:: {{title}}
authors:: {{authors}}{{directors}}
URL: [{{url}}]({{url}})
Zotero link: {{pdfZoteroLink}}

contribution:: 

# {{title}} 


{% if abstractNote %}
## Abstract
{{abstractNote}}
{% endif %}


## Annotations

### Important stuff

{% for a in annotations %}{% if a.annotatedText %}{% if a.colorCategory == "Red" %} >{{a.annotatedText}}{% endif %}{% endif %}{% endfor %}


### Notes 
{% for a in annotations %}{% if a.annotatedText %}{% if a.colorCategory == "Yellow" %}
```{{a.annotatedText}}```
{% endif %}{% endif %}{% endfor %}

## Knowledge to check
{% for a in annotations %}{% if a.annotatedText %}{% if a.colorCategory == "Green" %}
- [ ] {{a.annotatedText}}
{% endif %}{% endif %}{% endfor %}

