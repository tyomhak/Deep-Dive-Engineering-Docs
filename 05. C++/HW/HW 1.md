[Solution link](https://github.com/tyomhak/EngineeringDeepDive/blob/main/Cpp/01/Homework_01.cpp)
#### Problem 1
Write a function template, which will print content of provided `std::vector<>` to the console. 
If it is vector of integers, an example output is:
`[5, 32, 14, 6]`
#### Problem 2
Write its specialization for printing vector of strings, so every string will be double-quoted. Example output is:
`["hello", "kitty", "move", "on"]`

#### Problem 3
Write another specialization for printing vector of characters, which will print every character in single quotes. 
Example:
`['f', 'h', 'Z', 'X']`

#### Problem 4
Finally, write a specialization for printing vector of `std::pair<>` objects. In that case, each pair should appear in brackets. 
If the vector consists of pairs of strings and integers, then example output is:
`[(h:22), (ptr:7), (key:84)]`
