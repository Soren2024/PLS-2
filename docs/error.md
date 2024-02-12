# Error handling

## General Rules
- Errors should be handled gracefully, providing clear and descriptive error messages to the user.
- Avoid using die() or exit() statements to handle errors.
- Use exceptions to handle errors whenever possible.
- Use error codes or error constants to identify specific errors.

## Exceptions
- Use built-in PHP exceptions or create custom exceptions to handle errors.
- Use try-catch blocks to catch and handle exceptions.
- Throw exceptions with descriptive messages to identify the source of the error.

## Error Reporting
- In development environments, set error_reporting to E_ALL and display_errors to On to ensure all errors are reported and displayed.
- In production environments, set error_reporting to E_ALL & ~E_NOTICE & ~E_DEPRECATED & ~E_STRICT and display_errors to Off to prevent sensitive information from being displayed to the user.
- Log errors to a file or database for future reference and debugging.

## Error Handling Functions
- Use built-in PHP error handling functions, such as set_error_handler() and set_exception_handler(), to customize error handling behavior.
- Avoid suppressing errors using the @ operator.

e.g:

```PHP
  ...
  catch(Exception $e)
  {
      if(DEBUG){
        echo 'Message: ' .$e->getMessage();
      }else{
        echo 'ERROR: Thank you for comforting me when I'm sad.';
      }
  }
```
