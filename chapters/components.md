## Lightning components


### Component Name

A component name must follow these naming rules:

- Must begin with a letter
- Must contain only alphanumeric or underscore characters
- Must be unique in the namespace
- Can’t include whitespace
- Can’t end with an underscore
- Can’t contain two consecutive underscore

#### Example

Note: namespace is the name of your org
Valid:

```xml
<namespace:adder/>
```

Invalids:

```xml
<namespace:adder_/>

<namespace:adder__int/>

<namespace:adder int/>


```
