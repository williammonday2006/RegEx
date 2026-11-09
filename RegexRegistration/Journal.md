# Phase 1

I created two functions using regular expressions to validate names and usernames. The start and end anchors make sure the entire username matches the required pattern instead of just checking part of it.

# Phase 2

I created phone and promo code validation functions. The phone regex checks for exactly 10 digits with optional separators. The case-insensitive flag makes it easier to accept different capitalization without converting the string manually.

# Phase 3

I created a function that uses capturing groups to separate phone numbers into three parts. I used replace() with backreferences to format valid numbers consistently. The test() method checks whether a string is valid, while capturing groups let me extract and reuse specific parts of a match.

# Phase 4

I created processRegistration() to combine all my validation functions. It checks each required field, collects errors, and returns either a failure message or sanitized registration data. Building the individual functions first made the final pipeline easier to organize and debug.