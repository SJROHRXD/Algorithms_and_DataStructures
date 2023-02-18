# Review and Refactor

## Refactoring Questions

- When you have a finished solution:
- Can you check the result?
- Can you derive the result differently?
- Can you understand it at a glance?
- Can you use the result or method for another problem?
- Can you improve the performance of your solution?
  - Time or Space Complexity, nested code, methods, etc???
- Can you think of other ways to refactor?
- How have other people solved this problem?

            function charCount(str) {
                var obj = {};
                for (var i = 0; i < str.length; i++) {
                    var char = str[i].toLowerCase;
                    if (/[a-z0-9]/.test(char)) {
                        if (ojb[char] > 0) {
                            obj[char]++;
                        } else {
                            obj[char] = 1;
                        };
                    }
                }
                return obj;
            }

Explained code:

This code defines a function charCount that takes a string str as input and returns an object that represents the count of each alphanumeric character in the string.

Declare an empty object obj that will store the character counts.

            var obj = {};

Loop through each character in the input string str, and convert it to lowercase.

            for (var i = 0; i < str.length; i++) {
                var char = str[i].toLowerCase();
                // ...
            }

Check if the current character is alphanumeric using a regular expression that matches lowercase letters and digits. If it is, increment the count of the character in the obj object. If the count is not yet initialized for the character, set it to 1.

            if (/[a-z0-9]/.test(char)) {
                if (obj[char] > 0) {
                    obj[char]++;
                } else {
                    obj[char] = 1;
                };
            }

Return the obj object containing the character counts.

            return obj;

Here's an example usage of the charCount function:

            var counts = charCount("Hello, World!");
            console.log(counts);
            // Output: { h: 1, e: 1, l: 3, o: 2, w: 1, r: 1, d: 1 }

In this example, the function returns an object that shows the count of each character that appears in the input string. The string "Hello, World!" contains one "h", one "e", three "l"s, two "o"s, one "w", one "r", and one "d". The counts are case-insensitive and do not include any non-alphanumeric characters.

### Pain Points:

- 'for' loop vs 'for of'
- maybe regX isn't as efficient / performance varies
- the if statement block is messy

            function charCount(str) {
                 var obj = {};
                 for (var char of str) {
                     char = char.toLowerCase();
                     if (/[a-z0-9]/.test(char)) {
                         obj[char] = ++obj[char] || 1;
                     }
                 }
                 return obj;
             }

- can maybe use character code, "a".charCodeAt(0)
- use a boolean comparison to improve performance

- The following code would be run on each character to improve performance:

            function isAlphaNumeric(char) {
                var code = char.charCodeAt(0);
                if (
                    !(code > 47 && code < 58) &&
                    !(code > 64 && code < 91) &&
                    !(code > 96 && code < 123)
                    ) {
                    return false;
                    }
                return true;
            }

            charCodeAt(0);

- Which would result in us changing our function:

            if (isAlphaNumeric(char)) {
                // then lowercase it
                // then obj char add or increment and so on
            }

- lowercase first or after? meh.
