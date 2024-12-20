# Unexpected Null Return in foo Function

This repository demonstrates a common JavaScript error involving unexpected null returns.  The `foo` function, while seemingly simple, exhibits unexpected behavior when one of its arguments is `null`. This is because the function directly returns `null` in that case.  This can lead to issues in applications if null values are not properly handled in the calling function.  The solution provided handles this gracefully by returning 0 instead of null. 

## Bug Description

The `foo` function is designed to add two numbers. However, if either of the inputs is `null`, it unexpectedly returns `null`.  Better error handling or a default value should be implemented.  The issue is that the function returns `null` which might not be expected in all cases. This could cause unexpected behavior in parts of an application that use the foo function without accounting for the potential null return.