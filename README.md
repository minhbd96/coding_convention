# Front End

## General

- [ ] Does the code work?
- [ ] Description of the project is included. (Link to backlog)
- [ ] Code is easily understand.
- [ ] Code is written following the coding standarts/guidelines (React in our case)
- [ ] Code is in sync with existing code patterns/technologies.
- [ ] DRY. Is the same code duplicated more than twice?
- [ ] Can the code be easily tested (don't forget about React components)?
- [ ] Are functions/classes/components reasonably small (not too big)?
- [ ] Event listeners removed at teardown.
- [ ] Naming conventions followed for variables, file names, translations.
- [ ] Separation of Concerns followed.

## Codestyle

- [ ] No hardcoded values, use constants values.
- [ ] Avoid multiple if/else blocks.
- [ ] No commented out code.
- [ ] No unnecessary comments: comments that describe the how.
- [ ] Add necessary comments where needed. Necessary comments are comments that describe the why.

## React code review

- [ ] Are components have defined propTypes?
- [ ] Keep components small.
- [ ] Functional components for components that don't use state. (maybe just remove it)
- [ ] No api calls in containers, delegate to Sagas
- [ ] No state updates in loop.
- [ ] No useless constructor.
- [ ] Minimize logic in the render method.
- [ ] Don’t use mixins, prefer HOC and composition.

## CSS/CSS in JS

- [ ] Consistent naming conventions are used (BEM, OOCSS, SMACSS, e.t.c.).
- [ ] CSS selectors are only as specific as they need to be; grouped logically.
- [ ] Use Hex color codes #000 unless using rgba().
- [ ] Avoid absolute positioning.
- [ ] Use flexbox.
- [ ] Avoid !important.
- [ ] Do not animate width, height, top, left and others. Use transform instead.
- [ ] Use same units for all project.
- [ ] Avoid inline styles.

## Others

- [ ] Same with the design
- [ ] Large amount of text won't break the layout
- [ ] Use ellipsis in case more than number of rows define in template(XD..)

# PHP Code

## General

- [ ] The code works
- [ ] The code is easy to understand
- [ ] Follows coding conventions
- [ ] Names are simple and if possible short
- [ ] Names are spelt correctly
- [ ] Names contain units where applicable
- [ ] There are no usages of [magic numbers](http://c2.com/cgi/wiki?MagicNumber)
- [ ] No hard coded constants that could possibly change in the future
- [ ] All variables are in the smallest scope possible
- [ ] There is no commented out code
- [ ] There is no dead code (inaccessible at Runtime)
- [ ] No code that can be replaced with library functions
- [ ] Variables are not accidentally used with null values
- [ ] Variables are immutable where possible
- [ ] Code is not repeated or duplicated
- [ ] No complex/long boolean expressions
- [ ] No negatively named boolean variables
- [ ] No empty blocks of code
- [ ] Ideal data structures are used
- [ ] Constructors do not accept null/none values
- [ ] Catch clauses are fine grained and catch specific exceptions
- [ ] Exceptions are not eaten if caught, unless explicitly documented otherwise
- [ ] Files/Sockets and other resources are properly closed even when an exception occurs in using them
- [ ] `null` is not returned from any method
- [ ] == operator and === (and its inverse !==) are not mixed up
- [ ] Floating point numbers are not compared for equality
- [ ] Loops have a set length and correct termination conditions
- [ ] Blocks of code inside loops are as small as possible
- [ ] No methods with boolean parameters
- [ ] No object exists longer than necessary
- [ ] No memory leaks
- [ ] Code is unit testable
- [ ] Test cases are written wherever possible
- [ ] Methods return early without compromising code readability
- [ ] Performance is considered
- [ ] Loop iteration and off by one are taken care of

## Architecture

- [ ] Design patterns if used are correctly applied
- [ ] [Law of Demeter](https://en.wikipedia.org/wiki/Law_of_Demeter) is not violated
- [ ] A class should have only a single responsibility (i.e. only one potential change in the software's specification should be able to affect the specification of the class)
- [ ] Classes, modules, functions, etc. should be open for extension, but closed for modification
- [ ] Objects in a program should be replaceable with instances of their subtypes without altering the correctness of that program
- [ ] Many client-specific interfaces are better than one general-purpose interface.
- [ ] Depend upon Abstractions. Do not depend upon concretions.

## API

- [ ] APIs and other public contracts check input values and fail fast
- [ ] API checks for correct oauth scope / user permissions
- [ ] Any API change should be reflected in the API documentation
- [ ] APIs return correct status codes in responses

## Logging

- [ ] Logging should be easily discoverable
- [ ] Required logs are present
- [ ] Frivolous logs are absent
- [ ] Debugging code is absent
- [ ] No `print_r`, `var_dump` or similar calls exist
- [ ] No stack traces are printed

## Documentation

- [ ] Comments should indicate WHY rather that WHAT the code is doing
- [ ] All methods are commented in clear language.
- [ ] Comments exist and describe rationale or reasons for decisions in code
- [ ] All public methods/interfaces/contracts are commented describing usage
- [ ] All edge cases are described in comments
- [ ] All unusual behaviour or edge case handling is commented
- [ ] Data structures and units of measurement are explained

## Security

- [ ] All data inputs are checked (for the correct type, length/size, format, and range)
- [ ] Invalid parameter values handled such that exceptions are not thrown
- [ ] No sensitive information is logged or visible in a stacktrace
