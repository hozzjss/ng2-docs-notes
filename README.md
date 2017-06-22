# ng2-docs-notes
## Template Syntax
* Template expressions and template statements

   > A template expression is about *getting* a value, and a template statement is about changing or *setting* a value through events.

## Expression guidelines

* No visible side effects: 
    > Don't set just get.

* Quick execution: 
    > Try to cache values that are the product of a slow function instead of re-executing the function over and over again.

* Simplicity: 
    > Don't do more than `!someVal`.

* Idempotence:
    > Just like pure functions same output for same input all the time.