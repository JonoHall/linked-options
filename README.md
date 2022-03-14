# Shopify's Dawn Theme Linked Options (drop down boxes only!)
This snippet generates linked options for Shopify's Dawn theme. Please note, this works for drop down boxes only, not the default "pill" selectors.

Development experience is required to use this snippet. This snippet is supplied "as-is", I cannot install/modify this snippet for your store. I am not personally affiliated with Shopify Inc.

### Example
Note the Box Quantity value changes from 36 to 12.

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
- Built in native javascript
- Automatically select an option if a variant is specified in the URL.
- Remove the variable parameter from the URL if an invalid selection is made.

## Disclaimer
This modification may contain bugs, it may stop working at any time, it is supplied completely "as-is". Please test this modification before making it live.

Install at your own risk, I accept no liability for any indirect or consequential loss or damage, or for any loss of data, profit, revenue or business if you install this modification.

## Say thanks!
Although this snippet is completely "as-is" and free for you to use/modify, if you are in the position to show a small token of thanks click the link below.

<a href="https://www.buymeacoffee.com/jonohallnz" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

Alternatively, "Star" this project or contribute!
