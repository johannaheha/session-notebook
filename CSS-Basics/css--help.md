
## 📋 CSS Selector Reference Table

| **Selector Type**          | **Syntax**        | **CSS Selector Example** | **HTML Example**                             | **Selected Elements**                       |
| -------------------------- | ----------------- | ------------------------ | -------------------------------------------- | ------------------------------------------- |
| **Type Selector**          | `element`         | `p`                      | `<p>This is a paragraph.</p>`                | `<p>` element                               |
| **Universal Selector**     | `*`               | `*`                      | `<div>Text</div><span>More text</span>`      | `<div>` and `<span>` elements               |
| **ID Selector**            | `#id`             | `#header`                | `<div id="header">Header</div>`              | `<div>` with `id="header"`                  |
| **Class Selector**         | `.class`          | `.highlight`             | `<span class="highlight">Text</span>`        | `<span>` with `class="highlight"`           |
| **Attribute Selector**     | `[attr]`          | `[disabled]`             | `<input disabled>`                           | `<input>` with `disabled` attribute         |
|                            | `[attr="value"]`  | `[type="text"]`          | `<input type="text">`                        | `<input>` with `type="text"`                |
|                            | `[attr~="value"]` | `[class~="highlight"]`   | `<div class="box highlight">Content</div>`   | `<div>` with `class` containing "highlight" |
|                            | `[attr\|="value"]` | `[lang\|="en"]`         | `<div lang="en-US">Text</div>`               | `<div>` with `lang="en-US"`                 |
|                            | `[attr^="value"]` | `[href^="https"]`        | `<a href="https://example.com">Link</a>`     | `<a>` with `href` starting "https"          |
|                            | `[attr$="value"]` | `[src$=".jpg"]`          | `<img src="photo.jpg">`                      | `<img>` with `src` ending ".jpg"            |
|                            | `[attr*="value"]` | `[data-info*="item"]`    | `<div data-info="item123">Data</div>`        | `<div>` with `data-info` containing "item"  |
| **Pseudo-class**           | `:hover`          | `button:hover`           | `<button>Click me</button>`                  | `<button>` while hovered                    |
| **Pseudo-element**         | `::before`        | `p::before`              | `<p>Text</p>`                                | Before the `<p>`'s content                  |
| **Combinator: Descendant** | (space)           | `div p`                  | `<div><p>Text</p></div>`                     | `<p>` inside `<div>`                        |
| **Combinator: Child**      | `>`               | `ul > li`                | `<ul><li>Item</li></ul>`                     | `<li>` directly under `<ul>`                |
| **Combinator: Adjacent**   | `+`               | `h1 + p`                 | `<h1>Title</h1><p>Text</p>`                  | `<p>` immediately after `<h1>`              |
| **Combinator: Sibling**    | `~`               | `h2 ~ p`                 | `<h2>Subtitle</h2><p>First</p><p>Second</p>` | Both `<p>`s after `<h2>`                    |
| **Grouping**               | `,`               | `h1, h2`                 | `<h1>Title</h1><h2>Subtitle</h2>`            | Both `<h1>` and `<h2>` elements             |

---


## 📋 CSS Pseudo-classes Reference Table

| **Pseudo-class**       | **CSS Selector Example**  | **HTML Example**                                    | **Selected Elements**                        |
| ---------------------- | ------------------------- | --------------------------------------------------- | -------------------------------------------- |
| `:active`              | `a:active`                | `<a href="#">Link</a>`                              | `<a>` when activated (e.g., clicked)         |
| `:any-link`            | `a:any-link`              | `<a href="url">Link</a>`                            | `<a>` with `href` attribute                  |
| `:autofill`            | `input:autofill`          | `<input type="text" value="Auto-filled">`           | `<input>` with autofilled value              |
| `:blank`               | `p:blank`                 | `<p>   </p>`                                        | `<p>` with no content (including whitespace) |
| `:checked`             | `input:checked`           | `<input type="checkbox" checked>`                   | Checked `<input>`                            |
| `:default`             | `input:default`           | `<input type="radio" checked>`                      | Default selected `<input>`                   |
| `:defined`             | `custom-element:defined`  | `<custom-element></custom-element>`                 | Defined custom elements                      |
| `:disabled`            | `input:disabled`          | `<input type="text" disabled>`                      | Disabled `<input>`                           |
| `:empty`               | `div:empty`               | `<div></div>`                                       | `<div>` with no children                     |
| `:enabled`             | `input:enabled`           | `<input type="text">`                               | Enabled `<input>`                            |
| `:first-child`         | `li:first-child`          | `<ul><li>First</li><li>Second</li></ul>`            | First `<li>` in `<ul>`                       |
| `:first-of-type`       | `p:first-of-type`         | `<div><p>First</p><p>Second</p></div>`              | First `<p>` in `<div>`                       |
| `:fullscreen`          | `video:fullscreen`        | `<video></video>` (in fullscreen mode)              | `<video>` in fullscreen                      |
| `:focus`               | `input:focus`             | `<input type="text">`                               | `<input>` when focused                       |
| `:focus-visible`       | `button:focus-visible`    | `<button>Click me</button>`                         | `<button>` when focus is visible             |
| `:focus-within`        | `form:focus-within`       | `<form><input type="text"></form>`                  | `<form>` when any child has focus            |
| `:has()`               | `div:has(img)`            | `<div><img src="image.jpg"></div>`                  | `<div>` containing `<img>`                   |
| `:hover`               | `a:hover`                 | `<a href="#">Link</a>`                              | `<a>` when hovered                           |
| `:indeterminate`       | `input:indeterminate`     | `<input type="checkbox" indeterminate>`             | Indeterminate `<input>`                      |
| `:in-range`            | `input:in-range`          | `<input type="number" min="1" max="10" value="5">`  | `<input>` within range                       |
| `:invalid`             | `input:invalid`           | `<input type="email" value="invalid">`              | Invalid `<input>`                            |
| `:is()`                | `:is(h1, h2, h3)`         | `<h2>Heading</h2>`                                  | `<h2>` element                               |
| `:lang()`              | `p:lang(en)`              | `<p lang="en">Hello</p>`                            | `<p>` with `lang="en"`                       |
| `:last-child`          | `li:last-child`           | `<ul><li>First</li><li>Second</li></ul>`            | Last `<li>` in `<ul>`                        |
| `:last-of-type`        | `p:last-of-type`          | `<div><p>First</p><p>Second</p></div>`              | Last `<p>` in `<div>`                        |
| `:link`                | `a:link`                  | `<a href="url">Link</a>`                            | Unvisited `<a>`                              |
| `:not()`               | `div:not(.active)`        | `<div class="inactive">Content</div>`               | `<div>` not with class "active"              |
| `:nth-child(n)`        | `li:nth-child(2)`         | `<ul><li>First</li><li>Second</li></ul>`            | Second `<li>` in `<ul>`                      |
| `:nth-last-child(n)`   | `li:nth-last-child(1)`    | `<ul><li>First</li><li>Second</li></ul>`            | Last `<li>` in `<ul>`                        |
| `:nth-of-type(n)`      | `p:nth-of-type(2)`        | `<div><p>First</p><p>Second</p></div>`              | Second `<p>` in `<div>`                      |
| `:nth-last-of-type(n)` | `p:nth-last-of-type(1)`   | `<div><p>First</p><p>Second</p></div>`              | Last `<p>` in `<div>`                        |
| `:only-child`          | `p:only-child`            | `<div><p>Only child</p></div>`                      | `<p>` if it's the only child of `<div>`      |
| `:only-of-type`        | `p:only-of-type`          | `<div><p>Only</p></div>`                            | `<p>` if it's the only `<p>` in `<div>`      |
| `:optional`            | `input:optional`          | `<input type="text">`                               | Optional `<input>`                           |
| `:out-of-range`        | `input:out-of-range`      | `<input type="number" min="1" max="10" value="15">` | `<input>` out of range                       |
| `:placeholder-shown`   | `input:placeholder-shown` | `<input type="text" placeholder="Enter text">`      | `<input>` showing placeholder                |
| `:read-only`           | `input:read-only`         | `<input type="text" readonly>`                      | Read-only `<input>`                          |
| `:read-write`          | `input:read-write`        | `<input type="text">`                               | Editable `<input>`                           |
| `:required`            | `input:required`          | `<input type="text" required>`                      | Required `<input>`                           |
| `:root`                | `:root`                   | `<html>...</html>`                                  | `<html>` element                             |
| `:scope`               | `:scope`                  | `<div><p>Paragraph</p></div>`                       | `<div>` as the reference point               |
| `:target`              | `#section1:target`        | `<div id="section1">Section 1</div>`                | `<div>` when targeted via URL fragment       |
| `:valid`               | `input:valid`             | `<input type="email" value="user@example.com">`     | Valid `<input>`                              |
| `:visited`             | `a:visited`               | `<a href="url">Link</a>`                            | Visited `<a>`                                |
| `:where()`             | `:where(h1, h2, h3)`      | `<h1>Heading</h1>`                                  | `<h1>` element                               |

---

## 📋 CSS Pseudo-elements Reference Table

| **Pseudo-element** | **CSS Selector Example**     | **HTML Example**                                             | **Selected Elements**                                  |
| ------------------ | ---------------------------- | ------------------------------------------------------------ | ------------------------------------------------------ |
| `::after`          | `p::after`                   | `<p>Text</p>`                                                | Inserts content **after** `<p>`’s text                 |
| `::before`         | `p::before`                  | `<p>Text</p>`                                                | Inserts content **before** `<p>`’s text                |
| `::first-letter`   | `p::first-letter`            | `<p>Paragraph text.</p>`                                     | The first letter of the `<p>`’s text                   |
| `::first-line`     | `p::first-line`              | `<p>Paragraph text on one line.</p>`                         | The first line of the `<p>`’s text (depends on layout) |
| `::selection`      | `p::selection`               | `<p>Selectable text</p>`                                     | The text highlighted when selected                     |
| `::backdrop`       | `dialog::backdrop`           | `<dialog open>Modal content</dialog>`                        | The backdrop behind the modal dialog                   |
| `::marker`         | `li::marker`                 | `<ul><li>Item 1</li></ul>`                                   | The bullet or marker of the `<li>`                     |
| `::placeholder`    | `input::placeholder`         | `<input type="text" placeholder="Enter text">`               | The placeholder text inside the `<input>`              |
| `::cue`            | `video::cue`                 | `<video><track src="captions.vtt" kind="subtitles"></video>` | Subtitle cue lines inside `<video>`                    |
| `::spelling-error` | `textarea::spelling-error`   | `<textarea>Misspelled wrod</textarea>`                       | Misspelled words flagged by the browser                |
| `::grammar-error`  | `textarea::grammar-error`    | `<textarea>Incorrect grammar</textarea>`                     | Grammar errors flagged by the browser                  |
| `::part(name)`     | `custom-element::part(name)` | `<custom-element><div part="name"></div></custom-element>`   | The named part of the shadow DOM (when supported)      |

### 🔎 Notes

✅ Most pseudo-elements are **styling hooks** that let you target **parts of elements** that aren’t part of the direct DOM structure.
✅ Some (like `::before` and `::after`) let you **inject content** using `content:` in CSS.
✅ Others (like `::selection` or `::placeholder`) style **browser-generated or user-interaction elements**.
