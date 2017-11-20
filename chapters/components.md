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
   <td> <pre>c:myComponent</pre> </td>
   <td><pre> namespace:myComponent </pre></td>
 </tr>

 <tr>
   <td>Component used in system attribute	</td>
   <td> <pre> aura:component extends="c:myComponent" </pre></td>
    <td><pre>  aura:component extends="namespace:myComponent"</pre></td>
 </tr>

 <tr>
   <td>Component used in system attribute	</td>
   <td><pre>  aura:component implments="c:myInterface"</pre> </td>
    <td><pre>  aura:component implments="namespace:myInterface"</pre></td>
 </tr>

</table>

[More examples](https://developer.salesforce.com/docs/atlas.en-us.lightning.meta/lightning/namespace_using_reference.htm)


### Component Bundles

A component bundle contains a component or an app and all its related resources

<table>
<tr>
<td> Application or Component : </td>
<td>MyApp.app or myComponent.cmp : </td>
<td>The required resource in the component bundle. Each bundle contains only one component or app resource </td>
</tr>

<tr>
  <td>CSS styles : </td>
  <td>myComponent.css : </td>
  <td>contains the styles for the component </td>
</tr>

<tr>
<td>Controller : </td>
<td>myComponentController.js: </td>
 <td> Client-side controller methods to handle events in the component </td>
 </tr>


<tr>
  <td>Helper     : </td>
  <td> myComponentHelper.js </td>
  <td>: contains functions that can be called from any 
  JS code in the component's bundle </td>
</tr>

<tr>
<td>Design     : </td>
<td>myComponent.design: </td>
<td>Files required for the components used in App Builder, LX pages or Community Builder </td>
</tr>

<tr>
<td>Documentation: </td>
<td> myComponent.auradoc : </td>
<td>description, sample code to provide example of using this the component </td>
<td>
</tr>

<tr>
<td>Renderer: </td>
<td> myComponentRender.js : </td>
<td>Client-side renderer to override default rendering for a component
</td></tr>

<tr>
<td>SVG file:
</td><td>myComponent.svg:
</td><td>Custom Icon for component used in the App Builder or Community Builder
</td>
</tr>
</table>
------
All resources in the component bundle follow the naming convention and are auto-wired. For example, a controller <componentName>Controller.js is auto-wired to its component, which means that you can use the controller within the scope of that component. In above example: componentName = myComponent
