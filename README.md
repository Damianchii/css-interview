
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
> * Avoid Selectors That Are Too Broad - Overly broad selectors (e.g., *, `body` *) can cause unnecessary performance hits as they require more processing power for styling. Be specific with your selectors to target only the necessary elements.
> * <b> Minimize the Use of `!important`</b> - While !important can override specificity, its excessive use can lead to specificity wars and make debugging and maintaining styles more difficult.
> * <b>Reduce Nesting </b> - Deeply nested selectors increase specificity and can make CSS harder to read and maintain. Try to keep your CSS as flat as possible.
> * <b>Use Shorthand Propertiesc </b> - Shorthand properties like `margin`, `padding`, `font`, etc., can help reduce the size of your CSS files and improve readability.
> * <b>Optimize CSS Animations and Transitions</b> - Animations and transitions can be resource-intensive. Use hardware-accelerated properties (`transform` and `opacity`) and avoid animating properties that trigger layout reflows (`width`, `height`, etc.)
> * <b>Reduce Redundancy with Preprocessors</b> - CSS preprocessors like Sass and LESS allow you to use variables, mixins, and functions, reducing redundancy in your stylesheets and making them easier to maintain.
> * <b>Optimize Fonts</b> - Loading multiple fonts or large font files can slow down page rendering. Minimize the number of font files and their sizes, and consider using web-safe fonts or font subsets where possible.
> * <b>Use CSS Grid and Flexbox</b> - CSS Grid and Flexbox provide powerful layout capabilities without the need for complex float-based layouts. They can lead to cleaner, more efficient CSS.
> * <b>Optimize for Mobile</b> - Mobile devices often have limited resources, so it's essential to optimize your CSS for performance on smaller screens. Consider using media queries to serve different stylesheets or optimize existing styles for mobile.
> * <b>Leverage Browser Developer Tools</b> - Use browser developer tools to profile and debug your CSS for performance issues. Tools like Chrome DevTools provide insights into rendering times and layout thrashing.

> * Unikaj zbyt ogólnych selektorów - Zbyt ogólne selektory (np. *, body *) mogą powodować niepotrzebne spowolnienia wydajnościowe, ponieważ wymagają więcej mocy obliczeniowej do stylizacji. Bądź konkretny w wyborze selektorów, aby docelować tylko w niezbędne elementy.

> * <b>Zminimalizuj użycie !important</b> - Choć !important może zastąpić specyficzność, jego nadmierne stosowanie może prowadzić do wojen specyficzności i sprawić, że debugowanie oraz utrzymanie stylów będą trudniejsze.

> * <b>Zredukuj zagnieżdżenie</b> - Głęboko zagnieżdżone selektory zwiększają specyficzność i mogą sprawić, że CSS stanie się trudniejszy do czytania i utrzymania. Staraj się utrzymać swój CSS jak najpłaski.

> * <b>Używaj skróconych właściwości</b> - Skrócone właściwości, takie jak margin, padding, font, itp., mogą pomóc zmniejszyć rozmiar plików CSS i poprawić czytelność.

> * <b>Optymalizuj animacje i przejścia CSS</b> -  Animacje i przejścia mogą być zasobożerne. Używaj właściwości akcelerowane sprzętowo (transform i opacity) i unikaj animowania właściwości, które powodują reflowy układu (width, height, itp.).

> * <b>Zredukuj powtarzalność za pomocą preprocesorów</b> - Preprocesory CSS, takie jak Sass i LESS, pozwalają na korzystanie z zmiennych, mieszanych i funkcji, zmniejszając powtarzalność w arkuszach stylów i ułatwiając ich utrzymanie.

> * <b>Optymalizuj czcionki</b> -  Ładowanie wielu czcionek lub dużych plików czcionek może spowolnić renderowanie strony. Zminimalizuj liczbę plików czcionek i ich rozmiary oraz rozważ użycie czcionek internetowych lub ich podzbiorów, jeśli to możliwe.

> * <b>Używaj CSS Grid i Flexbox</b> - CSS Grid i Flexbox zapewniają potężne możliwości układu bez konieczności stosowania złożonych układów opartych na floatach. Mogą prowadzić do czystszego i bardziej wydajnego CSS.

> * <b>Optymalizuj pod kątem urządzeń mobilnych</b> -  Urządzenia mobilne często mają ograniczone zasoby, dlatego ważne jest zoptymalizowanie swojego CSS pod kątem wydajności na mniejszych ekranach. Rozważ stosowanie zapytań medialnych do dostarczania różnych arkuszy stylów lub optymalizację istniejących stylów pod kątem urządzeń mobilnych.

> * <b>Wykorzystaj narzędzia deweloperskie przeglądarek</b> - Użyj narzędzi deweloperskich przeglądarek do profilowania i debugowania swojego CSS pod kątem problemów wydajnościowych. Narzędzia takie jak Chrome DevTools dostarczają informacji na temat czasów renderowania i problemów z układem.
