# Input Kludge

`Input Kludge` is a probem in software design in which user input is not correctly handled. This term applies both to valid inputs being falsely rejected as well as bad input being accepted.

## Problems

Some of the largest breaches in enterprise security have been due to input kludge issues, when SQL was input into a user populated field and then executed on a server.

## Testing

The easiest and most simple test for input kludge is "facerolling" or "mashing" the keyboard to generate large garbage input. This is problematic for repeatability, however, and it is common to task UX engineers to attempt to cooerce the program to accept bad input. Automated testing using "fuzzing" generates random code snippets as well as random input to test against the input field. This is the most common practice when testing for Input Kludge.

## Solution

A common solution for Input Kludge is field Validation. Often the provided input is parsed through a series of regular expressions and algorithms to determine if it contains bad input before it is accepted and saved by the program. If the input is bad, it is rejected.
