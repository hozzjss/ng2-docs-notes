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

* Prohibited expressions
    > any sort of expression that might change state like : 
    
    > ```= ++ -- += -= new ; ,```
    
    > also Angular's template expression operators like `| ?.`

    > bitwise operators `& |`

## Binding Expressions
* From Component to view:
    
     > `{{ expression }} [target]="expression" bind-target="expression"`

* From view to component:
    > `(target)="expression" on-target="expression"`

* Two-way
    > `[(target)]="expression" bindon-target="expression"`

## Property Binding
* Attribute binding
    
    > Attribute binding creates a new attribute so if the attribute is not declared already it declares and sets it