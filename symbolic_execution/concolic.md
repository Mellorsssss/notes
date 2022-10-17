### Concolic Execution
Concolic = Conc(rete) + (Symb)olic.

In terms of non-linear arithmetic or other expressions that common SMT solver could hardly solve, many path conditions' results are likely to be false, which leads to lower path coverage. 

In order to solve the problem above, concolic execution combines the concrete execution and symbolic execution together.Concolic execution begins with random test input.When concolic execution encouters some unfeasiable branch, it would negates last branch by invoking SMT solver to get a feasible solution to that branch.Since concolic could reserve variables that are hard to be represented symbolicly, coverage and efficiency is improved as a result.

### References
- [concolic tutorial](https://www.cs.cmu.edu/~aldrich/courses/17-355-19sp/notes/notes15-concolic-testing.pdf)