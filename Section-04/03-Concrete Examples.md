# Explore Concrete Examples

- Come up with concrete examples to better understand the problem
- Examples provide sanity checks (your eventual solution will work)
- User Stories!
- Unit Tests!

## Simple Examples

- Write down 2 or 3 simple examples with an input and output
- Easiest use cases
- Progress to more complex examples
- Explore edge cases
- Empty inputs
- Invalid inputs

### Write a function, which takes in a string, and returns counts of each character in the string

- charCount ("aaaa"), should return // {a:4}
- charCount ("hello"), // {h:1, e:1, l:2, o:1}

- NOTE: Right away, I'm thinking to myself, how did he determine that his return will be formatted that way // as in, character : number of characters in the given string

- Do we want to include letters that aren't there?
- Default set letters to zero? Clarify

- "my phone number is 999-9999" // what does this return look like?
- Do we want to account for spaces? Punctuation?
- Do we ignore casing? Consider Casing?

- What is returned if they didn't pass anything in? // empty string?
- Error handling?
- What if they passed in something that isn't a string // typeOf

- Validating input // Formatting output
