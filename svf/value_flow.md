### Memory Region
Kind of like the concept of object(from heap or stack).

### Memory SSA
There are two kinds of Memory SSA: chi and mu.chi represents the def and use of an object(i.e., from heap), while mu only represents the use of an object. These two kinds of ssa perform as side-effect annotation of how memory objects flow.They are inserted before stores and loads.Additionallly, mus are placed before mehtod call while chi are placed after method calls. At the beginning of a function, chi could be placed and at the end of a function, mu could be placed.

### Value-Flow Graph Construction
Connecting definations with uses, i.e., VFG nodes.VFG nodes could be gennerated from normal statements(copy, load, store etc.), callsite and function's entry/exit.