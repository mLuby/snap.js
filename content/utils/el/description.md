# Parameters

- `tagName`

  The new element's tag

- `attrs`

  A mapping of attribute names to values

- `children`

  A list of child nodes. A child can either be a string, or an HTML element (e.g. one generated by el())

# Examples

```
el('div', { id: 'my-div' }, [
  el('span', {}, ['Hello']),
  'World!',
])

/* The above results in the following HTML structure
<div id="my-div">
  <span>Hello</span>
  World!
</div>
*/
```
