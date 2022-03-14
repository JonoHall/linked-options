# Shopify's Dawn Theme Linked Options
Generates linked options for Shopify's Dawn theme.

# Installation
Add the following to "theme.liquid" just before the </body> tag:

```
    {% if(request.page_type == 'product') %}
    	{% render 'linked-options' %}
    {% endif %}
```

# Objectives
- Automatically select an option if a variant is specified in the URL.
- Remove the variable parameter from the URL if an invalid selection is made.
