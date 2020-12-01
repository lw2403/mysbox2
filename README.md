# Development - Mystery Shopping Website Architecture
# Organization of your components:
I have a component on the left for displaying the 12 items. And a component on the right is for displaying the shopping cart. 
The left parent component has 2 child components (card component & navbar component).
The right parent component has only 1 child component (card component).
So, I have 4 kinds of components in total. 

# How data is passed down through your component:
First, I set the value for the "props" of the child components by passing the parameter behind the tag name. (<Child paramterName = 'something' >) 
Then, I get the "props" value from the inside of the child components by this.props.parameterName.

# How user interactions can trigger changes in the state of components:
First, when the user clicked something, the call back function would be triggered. 
And then, the method of this.setState() could be invoked in that function body to change the value of the state.
