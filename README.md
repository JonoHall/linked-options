# Shopify's Dawn Theme Linked Options (drop down boxes only!)
Generates linked options for Shopify's Dawn theme. Please note, this works for drop down boxes only, not the default "pill" selectors.

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

## Background
I've been running a Shopify for 5+ years, due to the nature of our products, we require linked options. We've for our previous themes, we've used a modified version of Caroline Schnapp's linked-options solution. We wanted to switch to Shopify 2.0's Dawn theme, but Caroline's solution relies on jQuery which is no longer included with Shopifies theme.

Without a linked-option solution, we weren't able to move forward with this upgrade. My background is in backend development (PHP etc), I had no experience in Javascript, but have worked my way through this to come up with a stop-gap solution. So if there is something that looks odd to you Javascript devs, please feel free to submit a PR.

Hopefully this can be built out and improved for those that require linked-options.

## Disclaimer
This modification may contain bugs, it may stop working at any time.

Install at your own risk, I accept no liability for any indirect or consequential loss or damage, or for any loss of data, profit, revenue or business if you install this modification.

## Say thanks!
I spent a lot of time on this, and I'm passing this development time on to you, free of charge. However, if you are in the position to show a small token of thanks click the link below to make a small contribution.

<a href="https://www.buymeacoffee.com/jonohallnz" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

Alternatively, "Star" this project or contribute! It will motivate me to continue building/supporting this snippet.
