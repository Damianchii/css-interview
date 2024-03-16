
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

## ➡️ Describe BFC (Block Formatting Context) and how it works | Opisz BFC (Block Formatting Context) i jak on działa

> BFC (Block Formatting Context) in CSS is a mechanism that defines how block-level elements are laid out and interact with each other within a container. It ensures encapsulation, clearance of floats, and predictable block-level element alignment.

> BFC (Block Formatting Context) w CSS to mechanizm definiujący sposób układania elementów blokowych oraz ich interakcję wewnątrz kontenera. Zapewnia on izolację, usuwanie floatów oraz przewidywalne wyśrodkowanie elementów blokowych

## ➡️ What are the various clearing techniques and which is appropriate for what context? | Jakie są różne techniki oczyszczania i która jest odpowiednia w jakim kontekście?
> Currently, Grid and Flexbox techniques are preferred. "Floating" elements is becoming a thing of the past, while the "clearing" cleaning technique prevents problems related to `float` elements. For this we use, among others, `clear: both;`

> Aktualnie preferowane są techniki z użyciem Grid i Flexbox. "Floatowanie" elementów przechodzi już w zapomnienie, natomiast technika czyszczenia "clearing" zapobiega powstawania problemom związanym z elementami `float`. Używamy do tego m.in `clear: both;`

## ➡️ How would you approach fixing browser-specific styling issues? | Jak podszedłbyś do rozwiązywania problemów ze stylem specyficznych dla przeglądarki?

> * Use libraries like Bootstrap that already handles these styling issues for you.
> * Use `autoprefixer` to automatically add vendor prefixes to your code

> * Użyj bibliotek takich jak Bootstrap, które już rozwiązują za Ciebie te problemy ze stylizacją.
> * Użyj `autoprefixer`, aby automatycznie dodać `prefixy` do swojego kodu

## ➡️ How do you serve your pages for feature-constrained browsers | Jak udostępniasz swoje strony w przeglądarkach z ograniczonymi funkcjami

> * Graceful degradation — The practice of building an application for modern browsers while ensuring it remains functional in older browsers.
> * Progressive enhancement — The practice of building an application for a base level of user experience, but adding functional enhancements when a browser supports it.

> * Łagodna degradacja — praktyka tworzenia aplikacji dla nowoczesnych przeglądarek przy jednoczesnym zapewnieniu jej funkcjonalności w starszych przeglądarkach.
> * Progresywne ulepszanie — praktyka budowania aplikacji na podstawowym poziomie doświadczenia użytkownika, ale dodawanie ulepszeń funkcjonalnych, jeśli obsługuje je przeglądarka.

## ➡️ What are the different ways to visually hide content (and make it available only for screen readers) | Jakie są różne sposoby wizualnego ukrywania treści ?

> We can visually hide content by:
> * `visibility: hidden` 
> * `display: none;`

> Możemy wizualnie ukryć zawartość poprzez:
> * `visibility: hidden` 
> * `display: none;`

## ➡️ Have you ever used a grid system, and if so, what do you prefer? | Czy kiedykolwiek używałeś grid system, jesli tak , co wolisz ?
> I used `flex` and `grid` even though `float` is supported by older browsers

> Uzywałem `flex` i `grid` mimo ze `float` jest wspierany przez starsze przegladarki

## ➡️ Have you used or implemented media queries or mobile specific layouts/CSS? | Czy korzystałeś lub wdrażałeś `media queries` lub układy/CSS dostosowane do urządzeń mobilnych?
> Yes, i have. For example i'm transforming a stacked menu bar navigation into a fixed-bottom hamburger navigation

> Tak. Na przykład przekształcam skumulowaną nawigację na pasku menu w stałą nawigację po hamburgerze

## ➡️ Are you familiar with styling SVG? | Czy jesteś oznajomiony z SVG ?

> Yes, I use it a lot for icons

> Tak, często uzywam go do ikon

## ➡️ Can you give an example of an `@media` property other than `screen`? | Podaj przykad właściwości `@media` poza `screen`?

> Oprócz `screen`, istnieje kilka innych typów `@media` w CSS. 
> * `all` - style wewnątrz bloku `@media` all będą stosowane niezależnie od tego, czy strona jest wyświetlana na ekranie, drukowana czy oglądana na innym urządzeniu.
``` bash
@media all {
  body {
    background-color: lightgray;
  }
}
```
> * `print` - służy do stosowania stylów specyficznych dla drukowania

``` bash
@media print {
  /* Style specyficzne dla drukowania */
  body {
    font-size: 12px;
  }
  /* itd. */
}
```
> * `speech` - jest typem mediów w CSS, który jest stosowany do określania stylów dla urządzeń generujących mowę lub syntezę mowy, takich jak czytniki ekranowe.
``` bash
@media speech {
  .hide-for-speech {
    display: none;
  }
}
```

## ➡️ What are some of the "gotchas" for writing efficient CSS? | Jakie są "pułapki" w pisaniu wydajengo CSS ?
> 

