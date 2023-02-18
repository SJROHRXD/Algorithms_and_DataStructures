# Solve if you can OR Solve a simpler problem

## When You're Stuck

- Ignore the part you don't understand, and solve for what you currently know
- You can implement the difficult part afterwards
- Maybe, work on the core part of what should be returned, and add in the validation or exceptions afterwards

- Find core difficulty, ignore it, work on a simplified problem and find a solution, add difficulty back in

- If you can figure out how to handle it for one character or item or whatever, you can find a pattern
- Start with what you know

- If you forget a method, postpone it with pseudo code, and come back to it

            function charCount(str) {
                    // do something

                    // make object here

                    var result = {};

                    // loop over character in string

                    for (var i = 0; i < string.length; i++) {
                        var char = str[i].toLowerCase()
                        if (result[char > 0]) // it's already in there
                        result[char]++;
                    } else {
                        result[char] = 1;
                    };

                    // are there any of [this character] in our object already? *is it a key in object?
                    // if no, add character, set its count to one
                    // if yes, add +1 to character count

                    return result;

                    // return object w keys that are lowercase alphanumeric
                    // maybe string to lowercase befoooore
                    // var char = str[i] becomes var char = str[i].toLowerCase()
                    // non alphanumeric characters
                    // we could create an array with every valid character NO lol
                    // or we could use a regX; maybe ascii codes; I honestly think there's a method though
                    // add an additional if statement for the character validation and nest other else/if statement
            }

- \+ More Logic

            // if character is a number / letter, AND is in our object vs AND is NOT in our object
            // otherwise, if character is not number / letter, do nothing
