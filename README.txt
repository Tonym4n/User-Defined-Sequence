#User-Defined-Sequence
A program implementing a user defined sequence and its bidirectional iterator counterpart. 
Given a list of integers, builds and outputs a sequence of accumulated integers from the beginning to end and end to beginning (one per line) using iterators.
To be compiled via the command line with the usage: ./nums [-a] INTS_FILE_PATH
  where INTS_FILE_PATH specifies the path to a file containing only integers
  -a specifies the use of building the sequence with an array of fixed size 8
  if -a is not specified, builds the sequence using a doubly linked list

sample usages:
tonym4n@TPTM:~/User-Defined-Sequence$ ./nums
usage: ./nums [-a] INTS_FILE_PATH

tonym4n@TPTM:~/User-Defined-Sequence$ ./nums -a overflow-array.data
nums: arrayseq.hh:54: void ArraySeq<E>::push(const E&) [with E = std::__cxx11::basic_string<char>]: Assertion `index < maxSize && "arrayseq overflow"' failed.
Aborted (core dumped)

tonym4n@TPTM:~/User-Defined-Sequence$ ./nums overflow-array.data
1
9
2
8
3
7
4
6
5
5
6
4
7
3
8
2
9
1
