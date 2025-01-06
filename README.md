# ConcurrentModificationException in Java
This repository demonstrates a common error in Java, the `ConcurrentModificationException`.  The example code shows how this exception can be raised when modifying a collection while iterating over it with a for-each loop.  The solution showcases a safe way to modify the collection.

## Problem:
The provided code attempts to remove an element from an `ArrayList` while using a for-each loop for iteration. This approach leads to a `ConcurrentModificationException`.  The exception is thrown because the for-each loop uses an iterator internally which doesn't handle the concurrent modification.