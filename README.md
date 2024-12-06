# Incorrect Div Content Modification
This repository demonstrates a subtle bug related to modifying the content of a div element in HTML.  The `bug.html` file shows the incorrect approach using `textContent`, which removes any nested elements within the div. The `bugSolution.html` file shows the corrected approach using `innerHTML`, which preserves the nested structure.

## Bug Description
When directly replacing the content of a div element using `textContent`, any child elements (like paragraphs, spans, etc.) within that div are removed. This can lead to unexpected behavior if your intention is to modify the content while preserving the structure.

## Solution
The solution uses `innerHTML` to modify the content of the div. `innerHTML` allows you to replace the entire HTML content of the div, including any nested elements, giving you more control over the final output.