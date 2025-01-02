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