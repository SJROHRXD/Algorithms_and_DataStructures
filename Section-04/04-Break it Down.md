# Break // it // Down

## Communicate What You're Doing

- Verbalize steps you are going to take
- Explicitly write out steps, the basic components of solution
- Figure out any lingering questions or conceptual issues in this step

### Write a function, which takes in a string, and returns counts of each character in the string

- for this example, we are going to assume our interviewer only cares about alphanumeric characters and lowercase characters as well

- Type of skeleton of function or PSEUDO CODE:

            function charCount(str) {
                    // do something
                    // return
            }

            function charCount(str) {
                    // do something
                    // return an object w keys that are lowercase alphanumeric
            }

            function charCount(str) {
                    // do something
                    // loop over character in string
                    // make object
                    // return object w keys that are lowercase alphanumeric
            }

            function charCount(str) {
                    // do something

                    // make object here

                    // loop over character in string
                    // make lowercase*

                    // are there any of [this character] in our object already? *is it a key in object?
                    // if no, add character, set its count to one
                    // if yes, add +1 to character count

                    // return object w keys that are lowercase alphanumeric
            }

- \+ More Logic

            // if character is a number / letter, AND is in our object vs AND is NOT in our object
            // otherwise, if character is not number / letter, do nothing

## Assess Psuedo Code, Write Code.
