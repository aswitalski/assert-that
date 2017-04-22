# assert-that
JavaScript assertion library with super-simple syntax.

# Syntax

``` js
const node = shallowRender(template);

assert.that(node.firstChild.isElement().hasName('div').hasId());
assert.that(node.lastChild.isComponent(MyComponent).withChild(Element));

assert.that(element.children() > 5);
assert.that(element.children(MyComponent, { label: /Choose/ }) >= 1);

assert.that(component.services() == 3);
assert.that(component.services(OtherService));

assert.that(element.children().find(MyComponent, OtherComponent, 'div'));
assert.that(element.children().filter({ class: 'some-name' }) == 2);
```
