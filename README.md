### merge_fasta - an example of using Galaxy dataset collections

This tool is meant as an example of using [Galaxy](https://galaxyproject.org/) dataset collections. Two
modes are demonstrated: using a dataset collection as an input, and using a dataset as an input but
allowing multiple inputs to be specified. 

The two models are demonstrated individually in two branches - the `collection` branch is the first case,
a collection is given as input and iterated over (using the #for statement from the [Cheetah](http://www.cheetahtemplate.org/)
template language). The `multiple` branch uses dataset input with `multiple="true"` and thus allows
for either multiple individual inputs or a data collection. Appropriate test cases are provided for 
each - the `collection` cases uses `<element>` clauses that are rather like `<param>` clause in a
normal (single dataset) test case. The `multiple` case use a single input with the names separated by
commas to provide for . In the `master` branch these approaches are both provided and selected at runtime using a
conditional.
