# Haskell Bug: UnsafePerformIO in Pure Function

This repository demonstrates a common error in Haskell programming: the misuse of `unsafePerformIO` within a pure function. This violates Haskell's principles of referential transparency and can lead to unexpected and difficult-to-debug behavior.

The `bug.hs` file contains the buggy code, while `bugSolution.hs` offers a corrected version that avoids the unsafe operation and maintains purity.

**Key Concept:** Referential transparency ensures that a function's output depends solely on its inputs, with no side effects.  `unsafePerformIO` breaks this by introducing side effects into pure code. 