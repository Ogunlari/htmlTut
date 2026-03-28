Can you reformat to md for me, 
1. Universal Selector
2. and

* → selects all elements.

* {
  margin: 0;
  padding: 0;
}

2. Type (Element) Selector

Targets HTML elements by tag name.

p {
  color: blue;
}

3. Class Selector

Targets elements with a specific class.

.button {
  background-color: red;
}

4. ID Selector

Targets an element with a specific ID.

#header {
  font-size: 20px;
}

5. Attribute Selector

Targets elements with specific attributes.

input[type="text"] {
  border: 1px solid black;
}


Variants:

[attr] → has attribute

[attr=value] → exact value

[attr~=value] → contains word

[attr|=value] → starts with value

[attr^=value] → starts with value

[attr$=value] → ends with value

[attr*=value] → contains value

6. Grouping Selector

Applies same styles to multiple selectors.

h1, h2, h3 {
  font-family: Arial;
}

7. Combinators

Descendant (space) → selects descendants.

div p {
  color: green;
}


Child (>) → direct children only.

ul > li {
  list-style: none;
}


Adjacent sibling (+) → immediately after.

h1 + p {
  margin-top: 0;
}


General sibling (~) → any sibling after.

h1 ~ p {
  color: gray;
}

8. Pseudo-classes

Target elements in a specific state.

a:hover {
  color: red;
}


Common examples:

:hover, :focus, :active

:first-child, :last-child, :nth-child(n)

:not(selector) → negation

:checked, :disabled, :enabled

9. Pseudo-elements

Target a part of an element.

p::first-line {
  font-weight: bold;
}


Common examples:

::before, ::after

::first-line, ::first-letter

::placeholder

10. Combinational Selectors

Mix IDs, classes, elements, pseudo-classes/elements.

div#main.content > p:first-child {
  color: orange;
}
