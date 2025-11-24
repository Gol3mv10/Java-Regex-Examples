# Java-Regex-Examples


1. Email Check (Validation) 📧
Goal: To see if the text looks exactly like a proper email (e.g., user@domain.com).

The Big Idea: We use matches() to check the entire string against a pattern that requires a name part, an @ sign, and a domain part.

Simple Pattern: ^... @ ... $ (Must start and end correctly).


2. Find Digits (Extraction) 🔢
Goal: To pull out any number (like "12345") hidden inside a longer sentence.

The Big Idea: We use a Matcher with the find() loop to locate the pattern, piece by piece, anywhere in the text.

Simple Pattern: \\d+ (Find one or more digits).


3. Replace Spaces (Substitution) 🔄
Goal: To quickly change all spaces in a phrase into something else, like a hyphen.

The Big Idea: We use replaceAll() to find all matching spots and swap them out in one simple step.

Simple Pattern: \\s+ (Find one or more white spaces).


4. Password Check (Assertion) 🔒
Goal: To make sure a password is strong (e.g., at least 8 characters long AND has an uppercase, lowercase, and a number).

The Big Idea: We use special features called Lookaheads ((?=...)) that act like spies, checking for the required characters without actually "consuming" the characters, and then we check the total length.

Simple Pattern: It's complex, but it basically says: "Check for lower, check for upper, check for number, then check for 8+ total characters."
