# Unit testing applied theory

## Versions

PHP: >=8.1

## Initialisation

Initialise PHP unit.

Source files are available under `src/`

Namespace is `unit_test_application`

Create a PHPUnit XML file that includes this directory.

Tests should be made under the `tests/` folder.

## Stage 1

A calculator stand-alone Plain Old PHP Object (POPO). Use PHPUnit to test this
class ensuring a 100% coverage report.

Test for the following:

* Testing Happy Paths: Ensure each method works as expected with valid inputs.
* Edge Cases: Check for edge cases like division by zero.
* Exceptions: Verify the class throws exceptions as expected.

Provide 100% coverage in JUnit XML format.

Explain:

* Why JUnit coverage report is needed and useful
* What does 100% coverage mean?
* How to fake coverage, and why that's a bad thing...

## Stage 2

A `MessageProcessor` class that introduces Dependency Injection, allowing it to depend
on a separate service (`LoggerService`). 
The `LoggerService` is injected into the `MessageProcessor`, enabling easier 
testing and mocking.

Use *PHPUnit and Prophecy* to test the `MessageProcessor` class, 
ensuring a 100% coverage report.

Happy Paths:

* Ensure valid messages are processed correctly (e.g., converted to uppercase).
* Verify the logger is called with the correct message.

Edge Cases:

* Test for empty messages, ensuring appropriate logging and exception handling.

Interaction Testing:

* Validate the interactions between MessageProcessor and the injected LoggerService.

Exceptions:

* Confirm that processing an empty message throws an InvalidArgumentException.

How might the object be improved? How might testing assist with this?