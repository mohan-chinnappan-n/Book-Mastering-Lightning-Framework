### How to setup namespace for your org


#### About namespace

Namespace:

Every component is part of a namespace.
This is used to group related components together

Default namespace is 'c' 
Example: <c:adder/>

Referring:
Another component or application can reference a component
by adding <myNamespace:myComponent/>
Example: <mohansun:adder/>

LX components from SFDC has namespaces:
 aura
 ui
 force

How to set namespace for your org:

A namespace prefix:
    Distinguishes your package and its contents from those of other developers.
    Is unique across all salesforce.com organizations.
    Ensures your exclusive control of all package components.
    Automatically prepends to all components (custom objects, fields, and others).
    Never changes.




![Setup > Packages ] (./img/namespace/namespace-1.png)
![Setup > Packages ] (./img/namespace/namespace-2.png)
![Setup > Packages ] (./img/namespace/namespace-3.png)
![Setup > Packages ] (./img/namespace/namespace-4.png)
![Setup > Packages ] (./img/namespace/namespace-5.png)

### References

1. [Creating a Namespace in Your Organization ](https://developer.salesforce.com/docs/atlas.en-us.lightning.meta/lightning/namespaces_creating.htm)
