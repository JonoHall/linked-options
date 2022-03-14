# Shopify's Dawn Theme Linked Options
Generates linked options for Shopify's Dawn theme.

### Example
Note the Box Quantity value changes from 36 to 12).
https://user-images.githubusercontent.com/4916365/158121029-4500dbbc-95bc-4da5-85ea-60be14bee682.mp4

## Installation
1. Copy the "linked-selectors.liquid" file into the "snippets" section of your Dawn theme.
2. Add the following to "theme.liquid" just before the </body> tag:

```
    {% if(request.page_type == 'product') %}
    	{% render 'linked-options' %}
    {% endif %}
```

## Objectives
- Automatically select an option if a variant is specified in the URL.
- Remove the variable parameter from the URL if an invalid selection is made.
