frontend_developer_questions
============================

Questions that are asked in interviews for frontend developer positions


   * What's a hashtable?

      * A data structure used for associative arrays
   * What are undefined and undeclared variables?
   * What is a closure, and how/why would you use one?

      * This is when a inner variable is kept alive after the function has been executed (great for private variables)
   * 
      * Your favorite pattern used to create them? argyle (Only applicable to IIFEs)
   * Explain the "JavaScript module pattern" and when you'd use it.

      * anonymous, loose augmentation, private state, and sub-modules.
   * 
      * Bonus points for mentioning clean namespacing.
      * What if your modules are namespace-less?

   * How do you organize your code? (module pattern, classical inheritance?)

      * I like the module pattern though I also like being expressive with my JavaScript code and making it easy for programmers to look at the code and can easily add / subtract features that they need, thus I stick with functional inheritance. The module pattern is great for large applications that you don't want changed often
   * What's the difference between host objects and native objects?

      * native objects are objects what come with JavaScript (Date, Math, parseInt etc). host objects are things like window, history, getElementById as told my Eacma script
   * What's the difference between .call and .apply?

      * Apply parameters are elements in an array, where as .call uses standard variables when you don't know the length of the parameters being used
   * explain Function.prototype.bind?

      * allows you to use 'this' within child functions. Passing 'that' is much easier to understand
   * Explain "hoisting".

      * Variables are always hoisted to the top of the object/function that they are within
   * Describe inheritance patterns in JavaScript.

      * This is creating class like objects which contain a namespace for cleaner execution
   * Describe a strategy for memoization (avoiding calculation repetition) in JavaScript.

      * Call a function outside of a loop vs inside of it to eliminate the extra calculations every time by using a closure private variable to store a previous value to check against
   * What is the arity of a function?

      * Specifies the number of arguments expected by the function
      * replaced by the Function.prototype.length
   * What is "use strict";? what are the advantages and disadvantages to using it?

      * This strict context prevents certain actions from being taken and throws more exceptions.
      * 
         * It catches some common coding bloopers, throwing exceptions.
         * It prevents, or throws errors, when relatively "unsafe" actions are taken (such as gaining access to the global object).
         * It disables features that are confusing or poorly thought out.
         * It makes it harder to be expressive and free with coming up with new programs that access the global object
   * Explain "deferrers".

      * this is a way to ensure that all variables, objects, methods are available and/or finished when they are requested
   * What does .end() do?

      * It allows you to narrow down a selection based on the first set of selectors
   * How, and why, would you namespace a bound event handler?

      * namespacing events is used for readability, this is also useful when trying to remove all event handlers from similar or groups events
      * click.doSomethingCool vs click
   * What is the effects (or fx) queue?

      * Queues allow a sequence of actions to be called on an element asynchronously, without halting program execution.
   * What is the difference between .get(), [], and .eq()?

      * .get() and [0] returns the DOM element
      * .eq() returns a jquery object
   * What is the difference between $ and $.fn? Or just what is $.fn

      * $.fn points to the jQuery.prototype. Any methods or properties you add to it become available to all instance of the jQuery wrapped objects.$.something adds a property or function to the jQuery object itself.
Use the first form $.fn.something when you're dealing with DOM elements on the page, and your plugin does something to the elements. When the plugin has nothing to do with the DOM elements, use the other form $.something.

