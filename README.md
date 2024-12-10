# Scala Auxiliary Constructor Error
This repository demonstrates a common error in Scala related to auxiliary constructors.  Auxiliary constructors, which allow for multiple ways to initialize an object, must have the `this()` call to the primary constructor as their first statement.  Failure to do so results in a compile-time error. This example helps illustrate this pitfall and shows how to fix it.

## Bug:
The provided `MyClass.scala` file shows an attempt to create an auxiliary constructor that violates this rule; other statements are placed before the `this()` call, resulting in a compilation error.  The correct usage is to place the `this()` call first.

## Solution:
The `MyClassSolution.scala` file provides the corrected version, where the `this()` call is correctly placed at the beginning of the auxiliary constructor. The code now compiles and runs without errors.