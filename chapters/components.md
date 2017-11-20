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

<table>

 <tr>
   <th>Referenced Item</th>
   <th>With Default Namespace</th>
   <th>With Org Namespace</th>
 </tr>

 <tr>
   <td>Component used in markup	</td>
   <td> c:myComponent  </td>
   <td> namespace:myComponent </td>
 </tr>

 <tr>
   <td>Component used in system attribute	</td>
   <td> aura:component extends="c:myComponent" </td>
    td> aura:component extends="namespace:myComponent"</td>
 </tr>

 <tr>
   <td>Component used in system attribute	</td>
   <td> aura:component implments="c:myInterface" </td>
    td> aura:component implments="namespace:myInterface"</td>
 </tr>

</table>
