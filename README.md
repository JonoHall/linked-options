# Shopify's Dawn Theme Linked Options
Generates linked options for Shopify's Dawn theme.

# Installation
1. Copy the "linked-selectors.liquid" file into the "snippets" section of your Dawn theme.
2. Add the following to "theme.liquid" just before the </body> tag:

```
    {% if(request.page_type == 'product') %}
    	{% render 'linked-options' %}
    {% endif %}
```

# Objectives
- Automatically select an option if a variant is specified in the URL.
- Remove the variable parameter from the URL if an invalid selection is made.
