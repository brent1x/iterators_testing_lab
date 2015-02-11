##Descriptions of Iterators

###Instructions
Below you will find a list of methods. In the space provided below each, please provide a brief description of what this method does based upon your review of the Docs. 

###Array methods:
May be helpful to look in [Enumerable](http://ruby-doc.org/core-2.2.0/Enumerable.html) as well...

####select:

> **Select** returns an array for every element in an enumerable for which the given block of code returns a ~true~ value.

####reject:

> **Reject** returns an array for every element in an enumerable for which the given block of code returns a ~false~ value.

####map:

> **Map** returns a new array with the results of running the given block of code once for every element in the enumerable.

####detect:

> **Detect** passes each entry in an enumerable to the given block of code. It returns the first for which the block is ~not~ false. If no object passes, detect will call ifnone and returns its result when it is specified or returns nil otherwise. Appears that .find method is interchangeable with .detect method.

####inject:

> **Inject** combines all elements of an enumerable by applying a binary operation, specified by a given block of code or by a symbol that names a method or operator. If a block is specified, then for each element in the enumerator the block is passed an accumulator value. At the end of the iteration, the accumulator value is the return value for the method. Appears to be interchangeable with .reduce method.

####partition:

> **Partition** returns two arrays, the first containing the elements of the enumerable for which the given block of code evaluates to true, and the second array containing the remainder.

####sort:

> **Sort** returns an array containing the items in the enumerable sorted, according to their own <=> method, or by using the results as supplied by the given block of code.

####one:

> **One** passes each element of the collection to the given block of code. The method returns true *only* if the block returns true exactly once. If the block isn’t given, the method will only return true if exactly one member of the collection is true.

####none:

> **None** passes each element of the collection to the given block. The method returns true if the block never returns true for all of the elements. If the block is not given then none will return true *only* if none of the collection members is true.

####all:

> **All** passes each element of the collection to the given block of code. The method returns true if the block never returns false or nil. If the block isn’t given, Ruby adds an implicit block of { |obj| obj }, which will cause All to return true when none of the collection members are false or nil.

####empty?:

> **empty?** will return true if an array has a length of zero.

####eql?:

> **eql?** will return true if two arrays have the same length and content.

####include?:

> **include?** will return true if an array contains the given string or character.

####nil?:

> Only the object ~nil~ responds true to **nil?**

###Hash methods:

####key?:

> **key?** returns true if the given key is present in the hash.

####keys:

> **keys** will return a new array populated with the keys from this hash. See also: values.

####delete:

> **delete** will remove the key-value pair and return the values from the hash whose key is equal to key. If the key isn’t found, the method will return the default value. If the optional code block *is* given and the key is not found, pass in the key and return the result of the given block of code.

####delete_if:

> **delete_if** will delete every key-value pair from the hash for which the given block of code evaluates to true. If no block is given, an enumerator is returned instead.