##Easier Undo/Redo and Time Travel  
Immutability also makes some complex features mush easier to implement.For example ,further in this tutorial we will implement time travel between different stages of the game. Avoiding data mutations lets us keep a reference to older versions of the data,and switch between them if we need to
##Tracking Changes  
Determining if a mutated object has changed is complex because changes are made directly to the object.This then requires comparing the current object to a previous copy ,traversing the entire object tree ,and comparing each variable and value.this process can become increasingly complex.  
Determining how an immutable object has changed is considerably easier.if the object being referenced is different from before,then the object has changed , that's it.  
##Determining When to Re-render in React   
The biggest benefit of immutability in React comes when you build simple pure components.Since immutable data can more easily determin if changes have been made it also helps to determine when a component requires being re-rendered.  
To learn more about `shouldComponentUpdate()`and how you can build pure components take a look at Optimizing Performance.  
