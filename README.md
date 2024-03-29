
# 🚀 CSS Interview Questions 
<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=css" />
  </a>
</p>

## ➡️ What is CSS selector specificity and how does it work?
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

### Co to jest specyfikacja selektorów w CSS i jak ona działa?

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

## ➡️ What is the difference between "resetting" and "normalizing" CSS? Which would you choose, and why? 
> I will choose Reset to get a better look for the website, sacrificing compatibility and consistency.
> * Resetting CSS - Removes all default browser styling, requiring explicit styling for every element. 
> * Normalizing CSS - Preserves default browser styles while ensuring consistency across browsers.

### Jaka jest róznica pomiędzy "resetting" a "normalizing" w CSS? Co byś wybrał i dlaczego?

> Wybrałbym Reset żeby uzyskać lepszy wygląd strony, poświęcając kompatybilność i spójność
> * Resetting CSS - Usuwa wszystkie domyślne style przeglądarki, wymagając jawnego określenia stylów dla każdego elementu.
> * Normalizing CSS - Zachowuje domyślne style przeglądarki, zapewniając jednocześnie spójność między przeglądarkami.

## ➡️ Describe Floats and how they work 

> Floats in CSS are a layout technique used to position elements horizontally within a container. When an element is floated, it moves to the left or right of its container, allowing other elements to flow around it.

### Opis czym są Floaty i jak działają

> Floaty w CSS to technika układu używana do pozycjonowania elementów w poziomie wewnątrz kontenera. Kiedy element jest wyfloatowany, przesuwa się on w lewo lub w prawo względem swojego kontenera, pozwalając innym elementom na przepływanie wokół niego.

## ➡️ Describe `z-index` and how stacking context is formed 
> `z-index` in CSS determines the stacking order of positioned elements along the z-axis. It controls which elements appear in front of others when they overlap. stacking context is formed when an element is positioned (`relative`, `absolute`, or `fixed`) and has a `z-index` value other than `auto`, creating a new stacking context.

### Opisz `z-index` i sposób tworzenia stacking context

> `z-index` w CSS określa kolejność elementów wzdłuż osi z. Kontroluje, które elementy pojawią się na pierwszym planie, gdy zachodzi nakładanie się na siebie. stacking context jest tworzony, gdy element jest pozycjonowany (`relative`, `absolute` lub `fixed`) i ma wartość `z-index` inną niż `auto`, co powoduje utworzenie nowego kontekstu układania.

## ➡️ Describe BFC (Block Formatting Context) and how it works 

> BFC (Block Formatting Context) in CSS is a mechanism that defines how block-level elements are laid out and interact with each other within a container. It ensures encapsulation, clearance of floats, and predictable block-level element alignment.

### Opisz BFC (Block Formatting Context) i jak on działa

> BFC (Block Formatting Context) w CSS to mechanizm definiujący sposób układania elementów blokowych oraz ich interakcję wewnątrz kontenera. Zapewnia on izolację, usuwanie floatów oraz przewidywalne wyśrodkowanie elementów blokowych

## ➡️ What are the various clearing techniques and which is appropriate for what context?
> Currently, Grid and Flexbox techniques are preferred. "Floating" elements is becoming a thing of the past, while the "clearing" cleaning technique prevents problems related to `float` elements. For this we use, among others, `clear: both;`

### Jakie są różne techniki oczyszczania i która jest odpowiednia w jakim kontekście?

> Aktualnie preferowane są techniki z użyciem Grid i Flexbox. "Floatowanie" elementów przechodzi już w zapomnienie, natomiast technika czyszczenia "clearing" zapobiega powstawania problemom związanym z elementami `float`. Używamy do tego m.in `clear: both;`

## ➡️ How would you approach fixing browser-specific styling issues? 

> * Use libraries like Bootstrap that already handles these styling issues for you.
> * Use `autoprefixer` to automatically add vendor prefixes to your code

### Jak podszedłbyś do rozwiązywania problemów ze stylem specyficznych dla przeglądarki?

> * Użyj bibliotek takich jak Bootstrap, które już rozwiązują za Ciebie te problemy ze stylizacją.
> * Użyj `autoprefixer`, aby automatycznie dodać `prefixy` do swojego kodu

## ➡️ How do you serve your pages for feature-constrained browsers

> * Graceful degradation — The practice of building an application for modern browsers while ensuring it remains functional in older browsers.
> * Progressive enhancement — The practice of building an application for a base level of user experience, but adding functional enhancements when a browser supports it.

### Jak udostępniasz swoje strony w przeglądarkach z ograniczonymi funkcjami

> * Łagodna degradacja — praktyka tworzenia aplikacji dla nowoczesnych przeglądarek przy jednoczesnym zapewnieniu jej funkcjonalności w starszych przeglądarkach.
> * Progresywne ulepszanie — praktyka budowania aplikacji na podstawowym poziomie doświadczenia użytkownika, ale dodawanie ulepszeń funkcjonalnych, jeśli obsługuje je przeglądarka.

## ➡️ What are the different ways to visually hide content (and make it available only for screen readers) 

> We can visually hide content by:
> * `visibility: hidden` 
> * `display: none;`

### Jakie są różne sposoby wizualnego ukrywania treści ?

> Możemy wizualnie ukryć zawartość poprzez:
> * `visibility: hidden` 
> * `display: none;`

## ➡️ Have you ever used a grid system, and if so, what do you prefer? | Czy kiedykolwiek używałeś grid system, jesli tak , co wolisz ?
> I used `flex` and `grid` even though `float` is supported by older browsers

> Uzywałem `flex` i `grid` mimo ze `float` jest wspierany przez starsze przegladarki

## ➡️ Have you used or implemented media queries or mobile specific layouts/CSS? 
> Yes, i have. For example i'm transforming a stacked menu bar navigation into a fixed-bottom hamburger navigation

### Czy korzystałeś lub wdrażałeś `media queries` lub układy/CSS dostosowane do urządzeń mobilnych?

> Tak. Na przykład przekształcam skumulowaną nawigację na pasku menu w stałą nawigację po hamburgerze

## ➡️ Are you familiar with styling SVG? 

> Yes, I use it a lot for icons

### Czy jesteś oznajomiony z SVG ?

> Tak, często uzywam go do ikon

## ➡️ Can you give an example of an `@media` property other than `screen`? 

> Oprócz `screen`, istnieje kilka innych typów `@media` w CSS. 
> * `all` - style wewnątrz bloku `@media` all będą stosowane niezależnie od tego, czy strona jest wyświetlana na ekranie, drukowana czy oglądana na innym urządzeniu.
``` bash
@media all {
  body {
    background-color: lightgray;
  }
}
```
### Podaj przykad właściwości `@media` poza `screen`?

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

## ➡️ What are some of the "gotchas" for writing efficient CSS?
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

### Jakie są "pułapki" w pisaniu wydajengo CSS ?

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

## ➡️ What are the advantages/disadvantages of using CSS preprocessors?

> Advantages
> * <b>Increased Readability and Flexibility of Code</b> - Preprocessors allow the use of variables, functions, and nested selectors, which contribute to increased readability and flexibility of CSS code.
> * <b>Ability to Use Mixins and Functions</b> -Preprocessors enable the definition of mixins and functions, facilitating the repeated application of style sets and making code management easier.
> * <b>Ability to Divide Code into Modules</b> - Preprocessors make it easier to divide CSS code into modules, which facilitates managing large projects and collaboration among multiple developers.

> Disadvantages

> * <b>Additional Compilation Step</b> - Using preprocessors requires an additional compilation step to convert the code to plain CSS before deploying it to the server. This can add extra CPU overhead and prolong processing time.
> * <b>Unnatural Approach for Beginners</b> - For beginners, the syntax and conventions used in preprocessors may be slightly more complex and harder to understand compared to plain CSS.
> * <b>Need to Learn New Technology</b> - Using preprocessors requires learning new technology and familiarizing oneself with its syntax and capabilities, which can be time-consuming for developers already familiar with plain CSS.

### Jakie są korzyści i wady korzystania z preprocesorów CSS ?

> Korzyści
> * <b>Większona czytelność i elastyczność kodu</b> - Dzięki zastosowaniu preprocesorów możliwe jest używanie zmiennych, funkcji, a także zagnieżdżonych selektorów, co przyczynia się do zwiększenia czytelności i elastyczności kodu CSS.
> * <b>Możliwość używania mixinów i funkcji</b> -  Preprocesory umożliwiają definiowanie mixinów i funkcji, co pozwala na wielokrotne stosowanie zestawów stylów oraz ułatwia zarządzanie kodem.
> * <b>Możliwość dzielenia kodu na moduły</b> -  Dzięki preprocesorom łatwiej jest podzielić kod CSS na moduły, co ułatwia zarządzanie dużymi projektami i współpracę wielu programistów.

> Wady
> * <b> Dodatkowy etap kompilacji</b> - Korzystanie z preprocesorów wymaga dodatkowego kroku kompilacji kodu do zwykłego CSS przed umieszczeniem go na serwerze. Może to spowodować dodatkowe obciążenie procesora i wydłużyć czas pracy.
> * <b>Podejście nienaturalne dla początkujących</b> - Dla osób początkujących, składnia i konwencje stosowane w preprocesorach mogą być nieco bardziej skomplikowane i trudniejsze do zrozumienia w porównaniu do zwykłego CSS.
> * <b>Konieczność nauki nowej technologii</b> - Korzystanie z preprocesorów wymaga nauki nowej technologii i zapoznania się z jej składnią oraz możliwościami, co może być czasochłonne dla programistów, którzy są już zaznajomieni z czystym CSS.

## ➡️ Explain how a browser determines what elements match a CSS selector.

>A browser determines which elements match a CSS selector by traversing the Document Object Model (DOM) of the web page
> * <b>Selector Parsing</b> - Parsing the selector to understand its structure and components.
> * <b>Starting at the Root</b> - Starting at the root of the DOM tree.
> * <b>Traversing the DOM</b> - Iterating through each element in the DOM tree.
> * <b>Matching</b> - Checking if each element matches the selector based on its tag name, class, ID, attributes, and pseudo-classes specified in the selector.
> * <b>Applying Specificity and Inheritance</b> - Considering specificity and inheritance rules to determine the final styles applied to each matched element.

### Wyjaśnij jak przegladarka ustala jaki element pasuje do selektora w CSS

> Przeglądarka określa, które elementy pasują do selektora CSS, przeglądając Model Obiektowy Dokumentu (DOM) strony internetowej.
> * <b>  Analizę Selektora</b> - Analizę selektora w celu zrozumienia jego struktury i składników.
> * <b> Rozpoczęcie od Korzenia</b> - Rozpoczęcie od korzenia drzewa DOM.
> * <b> Przeglądanie DOM</b> - Przejście przez każdy element w drzewie DOM.
> * <b> Dopasowywanie</b> - Sprawdzenie, czy każdy element pasuje do selektora na podstawie jego nazwy tagu, klasy, identyfikatora, atrybutów i pseudoklas określonych w selektorze.
> * <b> Zastosowanie Specyficzności i Dziedziczenia</b> - Uwzględnienie zasad specyficzności i dziedziczenia w celu określenia końcowych stylów stosowanych do każdego dopasowanego elementu.

## ➡️ Describe pseudo-elements and discuss what they are used for.

> Pseudo-elements in CSS allow you to style specific parts of an element's content or structure.
> * `::before`: This pseudo-element allows content to be inserted before the element's content.
> * `::after` - Allows you to insert content after the content of the element
> * `::first-line` - This pseudo-element selects the first line of text within the element
> * `::first-letter` - Selects the first letter of the text inside the element
> * `::selection` - This pseudo-element reaches the text fragment selected by the user

### Opisz pesudo-element i przedyskutuj po co są używane 

> Pseudo-elementy w CSS pozwalają stylizować określone części zawartości lub struktury elementu.
> * `::before`: Ten pseudo-element umożliwia wstawianie zawartości przed zawartością elementu. 
> * `::after` - Umożliwia wstawianie zawartosci po zawartoscia elementu
> * `::first-line` - Ten pseudo-element wybiera pierwszą linię tekstu wewnątrz elementu
> * `::first-letter` - Wybiera pierwszą literę tekstu wewnątrz elementu
> * `::selection` - Ten pseudo-element dociera do zaznaczonego przez użytkownika fragmentu tekstu

## ➡️ Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
> The box model in CSS describes the layout of elements on a web page as rectangular boxes. Each box consists of content, padding, border, and margin areas, which together determine the size and spacing of the element.

> `box-sizing: content-box;` - Content-Box Model: In this model (the default), the width and height of an element apply only to its content area. Padding, border, and margin are added to the total dimensions of the element.

> `box-sizing: border-box;` - Border-Box Model: In this model, the width and height of an element include the padding and border, but not the margin. This means that the content area is adjusted to accommodate padding and border, and the specified width and height include these areas.

### Wyjaśnij jak rozumiesz box-model i jak powiedziałbyś przegladarce zeby wyrenderwoala layout w innym box model

> Model pudełkowy (box model) w CSS opisuje układ elementów na stronie internetowej jako prostokątne pudełka. Każde pudełko składa się z obszaru zawartości, wypełnienia (padding), obramowania (border) i marginesu, które razem określają rozmiar i odstępy elementu.

> `box-sizing: content-box;` - Model pudełkowy z zawartością (Content-Box) W tym modelu (domyślnym), szerokość i wysokość elementu dotyczą tylko jego obszaru zawartości. Wypełnienie, obramowanie i margines są dodawane do całkowitych wymiarów elementu.Czyli jesli damy width: 200px to sama zawartosc (`content`) bedzie miała 200px, do tego dodajemy `padding` `margin` `border`.

> `box-sizing: border-box;` - Model pudełkowy z obramowaniem (Border-Box) W tym modelu szerokość i wysokość elementu obejmują wypełnienie i obramowanie, ale nie margines. Oznacza to, że obszar zawartości jest dostosowany, aby pomieścić wypełnienie i obramowanie, a określona szerokość i wysokość obejmują te obszary. W tym przypadku jesli damy width 200px to cały `box` bedzie miał 200px lacznie z `margin` `border` `padding`

## ➡️ What is the CSS `display` property and can you give a few examples of its use?
>The CSS display property determines how an HTML element is displayed on the page.
> * `display: block` - The element is displayed as a block, which takes up the full available width on the page and starts on a new line. Examples of block-level elements are `<div>`, `<p>`, `<h1>`-`<h6>`.
> * `display: none` - The element is completely hidden and does not take up space on the page. 
> * `display: flex` - The element is displayed as a flex container, allowing for easy management of its children's layout.

### Co to jest właściwość `display` i podaj kilka przykładów ich użycia 

> Właściwość CSS display określa sposób, w jaki element HTML jest wyświetlany na stronie. 
> * `display: block` - Element jest wyświetlany jako blok, który zajmuje całą dostępną szerokość na stronie i zaczyna się od nowej linii. Przykładami blokowych elementów są `<div>`, `<p>`, `<h1>`-`<h6>`.
> * `display: none` - Element jest całkowicie ukryty i nie zajmuje miejsca na stronie
> * `display: flex` - Element jest wyświetlany jako element kontenerowy, który umożliwia łatwe zarządzanie układem jego dzieci

## ➡️ What is the difference between inline and inline-block?
> `inline` - The element is displayed inline, starting from the current line of text, without starting a new line. Examples of inline elements are `<span>`, `<a>`, `<strong>`.

> `inline-block` - The element is displayed like an inline element but retains block properties, such as the ability to set width and height. Examples of inline-block elements are `<img>`, `<button>`.

### Jaka jest roznica pomiedzy `inline` a `inline-block`?

> `inline` - Element jest wyświetlany w linii, zaczynając od bieżącej linii tekstu, bez rozpoczynania nowego wiersza. Przykładami elementów wyświetlanych inline są `<span>`, `<a>`, `<strong>`.

> `inline-block` - Element jest wyświetlany jak element inline, ale zachowuje właściwości blokowe, takie jak możliwość ustawienia szerokości i wysokości. Przykładami elementów inline-block są `<img>`, `<button>`.

## ➡️ What is the difference between the `nth-of-type()` and `nth-child()` selectors? 

> `nth-of-type()` - The `nth-of-type()` selector selects elements based on their position relative to other elements of the same type (same tag) within their container.
For example, `div:nth-of-type(2)` will select the second `<div>` element within its container.
> `nth-child()` - The `nth-child()` selector selects elements based on their position relative to all children of its container, regardless of their type (tag).
For example, `div:nth-child(2)` will select the second child of the container, whether it is `<div>`, `<p>`, or another element type.

### Jaka jest róznica pomiedzy `nth-of-type()` i `nth-child()` ?

> `nth-of-type()` - Selektor `nth-of-type()` wybiera elementy na podstawie ich pozycji względem innych elementów tego samego typu (tego samego tagu) w obrębie ich kontenera.
Na przykład `div:nth-of-type(2)` wybierze drugi element `<div>` w obrębie jego kontenera.
> `nth-child()` - Selektor `nth-child()` wybiera elementy na podstawie ich pozycji względem wszystkich dzieci swojego kontenera, niezależnie od ich typu (tagu).
Na przykład `div:nth-child(2)` wybierze drugie dziecko kontenera, niezależnie od tego, czy jest to `<div>`, `<p>`, czy inny typ elementu.

## ➡️ What is the difference between a relative, fixed, absolute and statically positioned element? 

> <b>`static`</b>

> * By default, HTML elements are statically positioned.
> * Statically positioned elements are positioned according to the normal flow of the document.
> * They are not affected by the top, right, bottom, or left properties.
> * Changing these properties on statically positioned elements has no effect.

> <b>`realtive`</b>

> * Elements with position: relative; are positioned relative to their normal position in the document flow.
> * They can be moved using the top, right, bottom, and left properties.
> * However, their new position does not affect the positions of other elements in the document flow.

> <b>`absolute`</b>

> * Elements with position: absolute; are removed from the normal document flow.
> * They are positioned relative to their closest positioned ancestor, if one exists; otherwise, they are positioned relative to the initial containing block.
> * Absolute positioned elements are not affected by the position of other elements.
> * They can be moved using the top, right, bottom, and left properties.

> <b>`fixed`</b>

> * Elements with position: fixed; are positioned relative to the viewport (the browser window).
> * They do not move when the page is scrolled.
> * Like absolute positioned elements, they are removed from the normal document flow.
> * Fixed positioned elements can be moved using the `top`, `right`, `bottom`, and `left` properties.

### Jaka jest różncia miedzy `relative` , `fixed` `absolute` `static`?

> <b>`static`</b>

> *Domyślnie elementy HTML mają pozycjonowanie statyczne.
> *Elementy statycznie pozycjonowane są rozmieszczane zgodnie z normalnym przepływem dokumentu.
> *Nie są one zmieniane przez właściwości top, right, bottom ani left.
> *Zmiana tych właściwości na elementach statycznie pozycjonowanych nie ma wpływu.

> <b>`realtive`</b>

> * Elementy z właściwością position: relative; są pozycjonowane względem ich normalnej pozycji w przepływie dokumentu.
> * Mogą być przemieszczane za pomocą właściwości top, right, bottom i left.
> * Jednak ich nowa pozycja nie wpływa na pozycje innych elementów w przepływie dokumentu.
> <b>`absolute`</b>

> * Elementy z właściwością position: absolute; są usuwane z normalnego przepływu dokumentu.
> * Są one pozycjonowane względem ich najbliższego przodka, który ma ustawioną pozycję, jeśli taki istnieje; w przeciwnym razie są one pozycjonowane względem początkowego bloku zawierającego.
> * Elementy pozycjonowane absolutnie nie są zmieniane przez pozycje innych elementów.
> *Mogą być one przemieszczane za pomocą właściwości top, right, bottom i left.

> <b>`fixed`</b>
> * Elementy z właściwością position: fixed; są pozycjonowane względem widoku (okna przeglądarki).
> * Nie przemieszczają się, gdy strona jest przewijana.
> * Podobnie jak elementy pozycjonowane absolutnie, są one usuwane z normalnego przepływu dokumentu.
> * Elementy pozycjonowane stałe mogą być przemieszczane za pomocą właściwości `top`, `right`, `bottom` i `left`.

## ➡️ What existing CSS frameworks have you used locally, or in production? How would you change/improve them?
> I often use Tailwindcss in my projects. Otherwise I am familiar with bootstrap

### Z jakich frameworków korzystałes ? 

> Często korzystam z Tailwind css w moich projektach. Poza tym jestem zeznajomiony z Bootstrap

## ➡️ Have you used CSS Grid?
> CSS Grid is used to design flexible, responsive, and precise web page layouts that adapt to various design needs and devices.

###  Używałeś CSS Grid ?

> CSS Grid jest używany do projektowania elastycznych, responsywnych i precyzyjnych układów stron internetowych, które dostosowują się do różnych potrzeb projektowych i urządzeń.

## ➡️ Can you explain the difference between coding a web site to be responsive versus using a mobile-first strategy?

> <b>Responsive Website Design</b>
> * Adapts the page layout to different screen sizes.
> * Typically starts with a desktop design and adapts for smaller screens using media queries.

> <b>Mobile-first</b>
> *Prioritizes design for mobile devices
> * Starts with design for small screens and gradually improves for larger ones
> * Focuses on simplicity, efficiency, and prioritizing relevant content for mobile users

### Czy możesz wytłumaczyć różnice między kodowaniem strony responsywnej a mobile-first ? 

> <b>Responsive Design Stron Internetowych</b>
> * Dostosowuje układ strony do różnych rozmiarów ekranu.
> * Zazwyczaj zaczyna się od projektowania dla komputerów stacjonarnych i dostosowuje dla mniejszych ekranów za pomocą zapytań medialnych.

> <b>Mobile-first</b>
> * Priorytetowo traktuje projektowanie dla urządzeń mobilnych
> * Rozpoczyna się od projektowania dla małych ekranów i stopniowo ulepsza dla większych
> * Koncentruje się na prostocie, wydajności i priorytetowaniu istotnej zawartości dla użytkowników mobilnych

## ➡️ Is there any reason you'd want to use `translate()` instead of `absolute` positioning, or vice-versa? And why? 

> I would choose `translate()` instead of `absolute` in animations. Translate are often hardware-accelerated by browsers, leading to smoother animations and better performance compared to absolute positioning, especially on mobile devices.

> And i would choose `absolute` when i need precise control over the exact position of an element relative

### Czy jest jakiś powód, dla którego chciałbyś używać funkcji translate() zamiast pozycjonowania bezwzględnego i odwrotnie? I dlaczego?

> W animacjach wybrałbym opcję `translate()` zamiast `absolute`. Tłumacze są często przyspieszane sprzętowo przez przeglądarki, co zapewnia płynniejsze animacje i lepszą wydajność w porównaniu z pozycjonowaniem bezwzględnym, szczególnie na urządzeniach mobilnych.

> Wybrałbym opcję `absolutną`, gdy potrzebuję precyzyjnej kontroli nad dokładnym położeniem elementu względnego

## ➡️ How is `clearfix` css property useful? 
> Yes it WAS useful but now when we have `flex` and `grid` we dont need to use `float`. It prevents the container from collapsing when it contains only floated elements

### Jak uzyteczny jest `clearfix` ?

> Tak BYŁ użyteczny ale teraz gdy mamy `flex` i `grid` nie potrzebujemy używać `float`. Zapobiega to zapadaniu się kontenera, gdy zawiera tylko "floatowane" elementy

## ➡️ Can you explain the difference between `px`, `em` and `rem` as they relate to font sizing? 

> <b>`px`</b>

> * `px` is an absolute unit of measurement commonly used in CSS.
> * It defines font size based on a fixed number of pixels, regardless of the parent or surrounding elements.
> * Font sizes specified in pixels do not change relative to the user's preferred font size settings in the browser.
> <b>`em`</b>

> * `em` is a relative unit of measurement based on the font size of the parent element.
> * When used to define font size, 1em is equivalent to the font size of the parent element.
> * For example, if the font size of the parent element is 16px, then 1em is equal to 16px.
> * Font sizes specified in em adjust dynamically based on changes in the font size of the parent element.
> <b>`rem`</b>

> * `rem` is a relative unit of measurement based on the font size of the root element (html).
> * When used to define font size, 1rem is equivalent to the font size of the root element.
> * Unlike em, which is relative to the font size of the parent element, rem is always relative to the font size of the root element.
> * Font sizes specified in rem are more predictable and easier to manage, especially in complex layouts with multiple nested elements.

### Czy potrafisz wyjasnic roznice pomiedzy `px` `em` i `rem` w odenisieniu do rozmiaru czcionki

> <b>`px`</b>

> * `px` to absolutna jednostka miary powszechnie stosowana w CSS.
> * Określa rozmiar czcionki na podstawie ustalonej liczby pikseli, niezależnie od elementu nadrzędnego lub otaczających elementów.
> * Rozmiary czcionek określone w pikselach nie zmieniają się względem preferowanych przez użytkownika ustawień rozmiaru czcionki w przeglądarce.

> <b>`em`</b>

> * `em` to jednostka miary względnej, oparta na rozmiarze czcionki elementu nadrzędnego.
> * Gdy używana jest do określania rozmiaru czcionki, 1em jest równy rozmiarowi czcionki elementu nadrzędnego.
> * Na przykład, jeśli rozmiar czcionki elementu nadrzędnego wynosi 16px, to 1em jest równy 16px.
> * Rozmiary czcionek określone w em dostosowują się dynamicznie do zmian rozmiaru czcionki elementu nadrzędnego.

> <b>`rem`</b>

> * `rem` to jednostka miary względnej, oparta na rozmiarze czcionki elementu korzenia (html).
> * Gdy używana jest do określania rozmiaru czcionki, 1rem jest równy rozmiarowi czcionki elementu korzenia.
> * W przeciwieństwie do em, które jest względne do rozmiaru czcionki elementu nadrzędnego, rem zawsze jest względne do rozmiaru czcionki elementu korzenia.
> * Rozmiary czcionek określone w rem są bardziej przewidywalne i łatwiejsze w zarządzaniu, szczególnie w skomplikowanych układach z wieloma zagnieżdżonymi elementami.

## ➡️ Can you give an example of a pseudo class? Can you provide an example use case for a pseudo class?

> In this example, `:hover` is the pseudo-class.
``` bash
a:hover {
  color: red;
}
```

### Czy możesz podać przykład pseudoklasy? Czy możesz podać przykładowy przypadek użycia pseudoklasy?

> To jest przykład pseudoklasy `:hover`.
``` bash
a:hover {
  color: red;
}
```

## ➡️ What is the difference between a block level element and an inline element. Can you provide examples of each type of element?

> block level element always starts in new line with full `width` available. Examples  `<div>`, `<p>`, `<h1>`.

> Inline level occupy only the necessary `width`, do not start on a new line. Examples `<span>`, `<a>`, `<strong>`.

### Jaka jest różnica między elementem blokowym a elementem wbudowanym. Czy możesz podać przykłady każdego typu elementu?

> element na poziomie bloku zawsze zaczyna się w nowej linii z dostępną pełną `width`. Przykłady `<div>`, `<p>`, `<h1>`.

> Poziom inline zajmuje tylko niezbędną `width`, nie zaczynaj od nowej linii. Przykłady `<span>`, `<a>`, `<strong>`.

## ➡️ What is the difference between CSS Grid and Flexbox? When would you use one over the other?
> CSS Grid is best suited for complex layouts involving both rows and columns, while Flexbox is great for aligning items within a single row or column.

### Jaka jest różnica między CSS Grid a Flexbox? Kiedy użyłbyś jednego zamiast drugiego?

> CSS Grid najlepiej sprawdza się w przypadku złożonych układów obejmujących zarówno wiersze, jak i kolumny, podczas gdy Flexbox świetnie nadaje się do wyśrodkowania elementów w jednym rzędzie lub kolumnie.

## ➡️ What is the difference between fixed, fluid and responsive layouts?
> `fixed`

> * The layout has fixed widths for its elements, typically specified in pixels.
> * Elements do not change size regardless of the screen size or device used.
> * The layout remains the same regardless of viewport size changes.

> `fluid`

> * The layout uses percentages for widths, allowing elements to resize relative to the viewport size.
> * Elements expand or contract based on the size of the viewport.
> * Provides some level of responsiveness but may not adapt optimally to all screen sizes.

> `responsive`

> * The layout adapts and responds to various screen sizes and devices.
> * It employs a combination of flexible grids, media queries, and fluid elements to adjust the design based on viewport size.
> * Elements may change their position, size, or visibility to provide the best user experience across different devices and screen resolutions.

### Jaka jest różnica między układami stałymi, płynnymi i responsywnymi?

> `fixed`

> * Układ ma stałe szerokości elementów, zazwyczaj określone w pikselach.
> * Elementy nie zmieniają rozmiaru niezależnie od wielkości ekranu lub urządzenia.
> * Układ pozostaje taki sam bez względu na zmiany wielkości widoku.

> `fluid`

> * Układ wykorzystuje procenty dla szerokości, pozwalając elementom zmieniać rozmiar w stosunku do wielkości widoku.
> * Elementy rozszerzają się lub kurczą w zależności od wielkości widoku.
> * Zapewnia pewien poziom responsywności, ale może nie dostosować się optymalnie do wszystkich wielkości ekranu.

> `responsive`

> * Układ dostosowuje się do różnych wielkości ekranów i urządzeń.
> * Wykorzystuje kombinację elastycznych siatek, zapytań medialnych i płynnych elementów, aby dostosować projekt w zależności od wielkości widoku.
> * Elementy mogą zmieniać swoje położenie, rozmiar lub widoczność, aby zapewnić najlepsze doświadczenie użytkownika na różnych urządzeniach i rozdzielczościach ekranu.
