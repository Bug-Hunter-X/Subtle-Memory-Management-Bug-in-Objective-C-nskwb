# Objective-C Memory Management Bug

This repository demonstrates a common and subtle memory management bug in Objective-C that can lead to crashes or unexpected behavior. The bug involves incorrect handling of object ownership using `retain`, `release`, and `autorelease`.

## Bug Description
The bug occurs when an object's property is set to another object which is then not properly released.  This can lead to a double release or the failure to release an object at all.  The solution demonstrates a correct implementation that avoids this issue.

## How to Reproduce
1. Clone the repository.
2. Open the `bug.m` file to see the flawed code.
3. Open the `bugSolution.m` file for the corrected version.
4. Compile and run the code (using Xcode or another Objective-C compiler).

## Solution
The corrected code in `bugSolution.m` shows how to correctly manage memory by ensuring proper release and avoid unnecessary retain cycles.

## Lessons Learned
This bug highlights the importance of careful memory management in Objective-C.  Understanding `retain`, `release`, `autorelease`, and how they interact is crucial for avoiding these kinds of errors.