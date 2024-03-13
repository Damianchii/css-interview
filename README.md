
# 🚀 CSS Interview Questions 
<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=css" />
  </a>
</p>

## ➡️ What is CSS selector specificity and how does it work? | Co to jest specyfikacja selektorów w CSS i jak ona działa?
> It determines which CSS rules take precedence when multiple rules apply to the same element. Specificity is calculated based on the components of a selector, such as element type, class, ID, and pseudo-classes/pseudo-elements.

> * Styles in the html tag line - specified using the `<style>` attribute
> * ID selectors in html tag - specified with id `<div id="name">Hello</div>`
> * Class selectors, attribute selectors and pseudo-classes - specified with:
> * * `class` - `<div class="name">Hello</div>`
> * * Attribute and pseudo-class selector - `a[href*="example.com"]{color: black}`
> * * `a:hover {color: red;}` pseudo-classes
> * Element selectors, pseudo-elements - these plot elements based on tag name or pseudo-elements, such as:
> * * `::after`
> * * `::before`

> Określa, które reguły CSS mają pierwszeństwo, gdy kilka reguł stosuje się do tego samego elementu. Specyficzność jest obliczana na podstawie składników selektora, takich jak typ elementu, klasa, ID oraz pseudoklasy/pseudoelementy.

> * Style w linii znacznika html - okreslane za pomoca atrybutu `<style>`
> * Selektory ID w znaczniku html - okreslane za pomoca id `<div id="name">Hello</div>`
> * Selektory class, selektory atrybutów i pseudoklasy - okreslane za pomoca :
> * * `class` - `<div class="name">Hello</div>` 
> * * Selektora atrybutu i pseudoklasy - `a[href*="example.com"]{color: black}`
> * * Pseudoklasy `a:hover {color: red;}`
> * Selektory elementów, pseudoelementy - kreślają one elementy na podstawie nazwy tagu lub pseudoelementów, takich jak :
> * * `::after`
> * * `::before`
