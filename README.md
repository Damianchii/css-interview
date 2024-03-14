
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
> * * `<h1>` , `<h2>` , `<p>`
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
> * * `<h1>` , `<h2>` , `<p>`
> * * `::after`
> * * `::before`

## ➡️ What is the difference between "resetting" and "normalizing" CSS? Which would you choose, and why? | Jaka jest róznica pomiędzy "resetting" a "normalizing" w CSS? Co byś wybrał i dlaczego?
> I will choose Reset to get a better look for the website, sacrificing compatibility and consistency.
> * Resetting CSS - Removes all default browser styling, requiring explicit styling for every element. 
> * Normalizing CSS - Preserves default browser styles while ensuring consistency across browsers.

> Wybrałbym Reset żeby uzyskać lepszy wygląd strony, poświęcając kompatybilność i spójność
> * Resetting CSS - Usuwa wszystkie domyślne style przeglądarki, wymagając jawnego określenia stylów dla każdego elementu.
> * Normalizing CSS - Zachowuje domyślne style przeglądarki, zapewniając jednocześnie spójność między przeglądarkami.

## ➡️ Describe Floats and how they work | Opis czym są Floaty i jak działają

> Floats in CSS are a layout technique used to position elements horizontally within a container. When an element is floated, it moves to the left or right of its container, allowing other elements to flow around it.

> Floaty w CSS to technika układu używana do pozycjonowania elementów w poziomie wewnątrz kontenera. Kiedy element jest wyfloatowany, przesuwa się on w lewo lub w prawo względem swojego kontenera, pozwalając innym elementom na przepływanie wokół niego.

## ➡️ Describe `z-index` and how stacking context is formed | Opisz `z-index` i sposób tworzenia stacking context

> `z-index` in CSS determines the stacking order of positioned elements along the z-axis. It controls which elements appear in front of others when they overlap. stacking context is formed when an element is positioned (`relative`, `absolute`, or `fixed`) and has a `z-index` value other than `auto`, creating a new stacking context.

> `z-index` w CSS określa kolejność elementów wzdłuż osi z. Kontroluje, które elementy pojawią się na pierwszym planie, gdy zachodzi nakładanie się na siebie. stacking context jest tworzony, gdy element jest pozycjonowany (`relative`, `absolute` lub `fixed`) i ma wartość `z-index` inną niż `auto`, co powoduje utworzenie nowego kontekstu układania.

## ➡️ 
