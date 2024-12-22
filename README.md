# F# Mutable Variable Bug

This repository demonstrates a common error in F# involving the unexpected behavior of mutable variables when passed to functions.  In F#, mutable variables are passed by reference. This means that any modifications made to the variables within a function directly affect the original variables outside the function.

The `bug.fs` file contains code that attempts to swap two mutable variables using a function, but due to the pass-by-reference nature, the swap doesn't work as intended.

The `bugSolution.fs` file provides a corrected version that uses a different approach to avoid this issue.