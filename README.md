# Objective-C Manual Memory Management (MRC) Bug: Double Release or Memory Leak

This repository demonstrates a common error in Objective-C's manual reference counting (MRC) memory management. The bug involves improper use of `retain` and `release`, leading to either a double-release (crash) or memory leaks.

The `bug.m` file showcases the erroneous code.  `bugSolution.m` provides the corrected version using `@property (nonatomic, copy) NSString *myString;` to avoid manual memory management.  This is highly recommended in modern Objective-C development.