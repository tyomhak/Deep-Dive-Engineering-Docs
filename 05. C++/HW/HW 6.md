[Solutions Link](https://github.com/tyomhak/EngineeringDeepDive/tree/main/Cpp/06/hw)

##### Part 1
1) Write a [metafunction](6.2%20CT%20Sequence%20Algorithms%201.md) for counting number of occurrences of given value 'Y', in provided [sequence](6.1%20CT%20Sequences.md).
##### Part 2
1) Write `ct_sequence_6` class template.
2) Implement `ct_sequence_L` class variadic template.

##### Part 3
Implement the following metafunctions:
1) `ct_pop_front< Seq >`, to remove first element of the sequence,
2) `ct_insert< Seq, Index, Value >`, to insert 'Value' in certain position,
3) `ct_erase< Seq, Index >`, to erase the value at position 'Index',
4) `ct_max_element< Seq >`, for computing maximal value of given sequence,
5) `ct_push_back< Seq, Value >`, for appending 'Value' to given sequence,
6) `ct_reverse< Seq >`, for reversing given sequence,
7) 'ct_insert_to_sorted< Seq, Value >', insertion of 'Value' into sorted sequence 'Seq', so the latter one will remain sorted
8) 'ct_insertion_sort< Seq >', implementation of sorting,

Advanced exercises:
1) Implement compile-time Binary search tree, and several metafunctions for it.