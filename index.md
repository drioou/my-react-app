#Easier Undo/Redo and Time Travel  
Immutability also makes some complex features mush easier to implement.For example,further in this tutorial we will implement time travel between different stages of the game. Avoiding data mutations lets us keep a reference to older versions of the data,and switch between them if we need to
#Tracking Changes
Determining if a mutated object has changed is complex because changes are made directly to the object.This then requires comparing the current object to a previous copy,traversing the entire object tree,and comparing each variable and value.this process can become increasingly complex.
