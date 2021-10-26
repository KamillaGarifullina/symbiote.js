# Symbi<span style="color:#f0f">ఠ</span>te.js

## 🥷 Ultralight and ultrapowerful library to create widgets, organize micro-frontends, build reusable embeddable components and libraries. Everything you need for your modern web application!

### 🔥 Core benefits
* Minimalistic but reach
* No additional dependencies
* Ultralight (2.6kb br/gzip for featurefull CDN version)
* Blazing fast (faster than most of the other mainstream solutions. All of them.)
* Memory friendly (no any redux-like immutables)
* CSP friendly - good for enterprize usage
* Highly extensible
* Easy to learn - nothing completely new for experienced developers, nothing complicated for newbies
* Works in all modern browsers. As is.
* Easy to test
* TypeScript friendly - use it in TS or JS projects from the common source code
* Integration friendly: works with any modern development stack
* Lifecycle control: no need to initiate something from outside
* ESM friendly - native JavaScript modules are best!
* Developer Experience on the mind: compact & convenient APIs, habitual syntax
* Open source (MIT license)

### 💎 Tech concept description
* Native `DocumentFragment` instead of expensive Virtual DOM sync
* Shadow DOM is optional. Use it when you need it only
* Styling approach: total freedom, from the old classics to the cutting age platforn abilities
* Native HTML and DOM API instead of expensive custom template syntax processing
* Templates are out of the component or render function context. It’s just a simple JavaScript template literals. So you can keep or process them wherever you want
* No logical operators in templates. Logic and presentation is strictly separated.
* Fast synchronous UI updates
* Full data context access from the document structure
* Full data context availability for template bindings
* DOM API friendly approach for the most perfomant solutions
* Convenient object model access instead of opaque abstractions
* Custom Elements work strange sometimes. Don’t worry about that, we do (construction flow)

### 🍏 Quick start
Easiest way to try Symbiote.js is to create simple `html` file in your text editor and connect the Symbiote base class from CDN:

```html
<script type="module">
  import { BaseComponent } from 'https://uc-jsdk.web.app/build/symbiote.js';

  class MyComponent extends BaseComponent {
    init$ = {
      count: 0,
      increment: () => {
        this.$.count++;
      },
    }
  }

  MyComponent.template = /*html*/ `
    <h2 set="textContent: count"></h2>
    <button set="onclick: increment">Click me!</button>
  `;

  MyComponent.reg('my-component');
</script>

<my-component></my-component>
```

**This code can work directly in any modern browser, so you don't need to install anything to try it!**

## 🧜‍♀️ Dive deeper
* [Templates](https://github.com/uploadcare/symbiote.js/blob/main/docs/Templates.md)
* [Lifecycle](https://github.com/uploadcare/symbiote.js/blob/main/docs/Lifecycle.md)
* [Component data context](https://github.com/uploadcare/symbiote.js/blob/main/docs/Component_data_context.md)
* [Attribute binding](https://github.com/uploadcare/symbiote.js/blob/main/docs/Attribute_binding.md)
* [Extending](https://github.com/uploadcare/symbiote.js/blob/main/docs/Extending.md)
* [Naming collisions](https://github.com/uploadcare/symbiote.js/blob/main/docs/Naming_collisions.md)
* Data (pub/sub)
* Routing
* Domain specific data
* DOM helpers
* Indexed DB
* Solution history
* Playground

## ✅ Browser support
Symbiote.js is supported and tested in all major modern desktop and mobile browsers: 
* Chrome
* Firefox
* Safari
* Edge
* Opera
* etc...

**Internet Explorer** - is outdated and not supported anymore:

https://uploadcare.com/blog/uploadcare-stops-internet-explorer-support/

(But it's possible with polyfills: https://github.com/webcomponents/polyfills/tree/master/packages/webcomponentsjs)

## 💰 General sponsor
Big thanks to 🟡 **Uploadcare** for supporting this project!

> https://uploadcare.com/

## Symbiote widget example
https://github.com/uploadcare/jsdk/tree/main/upload-blocks

### 🌎 Useful external links:
* https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_custom_elements
* https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM
* https://custom-elements-everywhere.com
* https://open-wc.org/

## This is not a final version of the README file, work still in progress...

## Issues and PRs are welcome
