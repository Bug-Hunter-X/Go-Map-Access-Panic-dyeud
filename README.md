# Go Map Access Panic

This repository demonstrates a common error in Go: panicking when accessing a map with a non-existent key.  The `bug.go` file shows the erroneous code, while `bugSolution.go` provides a corrected version.

The problem arises because Go's maps don't return an error when a key is not found; instead, attempting to access a non-existent key results in a runtime panic.  This can make debugging difficult, especially in complex applications.

The solution involves checking if the key exists before accessing it using the `ok` idiom, ensuring the program handles the case gracefully.
