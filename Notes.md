
# Errors
* Prefer using `.expect` over `.unwrap` in production code  
* To avoid excessive `match` statements we can use `.unwrap_or_else`
* Errors can be propogated up the call stack by placing the `?` operator at the end of an expression
    * If the expression returns an `Ok()` then the function will continue
    * If the expressions return an `Err()` then the function will return 