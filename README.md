# SauceDemo Manual Testing

Manual testing project on the SauceDemo e-commerce demo site (saucedemo.com), done entirely on an Android phone with Chrome.

## Summary
- 43 test cases designed and executed
- 37 passed, 6 failed (86% pass rate)
- 7 defects logged with severity, priority, steps to reproduce and evidence

## Scope
Login, Products page (listing, sorting, product details), Cart, Checkout, Logout and session handling, and the special test users (locked_out_user, problem_user, performance_glitch_user, error_user).

## Test techniques used
- Positive and negative testing
- Boundary value analysis and equivalence partitioning
- UI and usability checks
- Exploratory testing with problem and error users

## Defects found
| Bug ID | Summary | Severity | Evidence |
|---|---|---|---|
| BUG_001 | Long login error message is clipped in the red banner on mobile | Low | [screenshot](BUG_001.jpg) |
| BUG_002 | All products show the same image for problem_user | Medium | [screenshot](BUG_002.jpg) |
| BUG_003 | Last Name cannot be typed on checkout for problem_user | High | [screenshot](BUG_003.jpg) |
| BUG_004 | Add to cart and Remove fail on some products for problem_user | High | [screenshot](BUG_004.jpg) |
| BUG_005 | Finish button does nothing for error_user, order cannot complete | Critical | [screenshot](BUG_005.jpg) |
| BUG_006 | Sorting does nothing for problem_user | Medium | none (the screen did not change) |
| BUG_007 | Checkout continues without a Last Name for error_user | High | [screenshot](BUG_005.jpg) |

## Files
- `SauceDemo_Test_Log.xlsx`: test cases, bug reports and summary sheets
- `BUG_001.jpg` to `BUG_005.jpg`: screenshots for the bugs (BUG_005.jpg also covers BUG_007)

## Tools and concepts
Manual testing, test case design, defect reporting, severity vs priority, STLC.
