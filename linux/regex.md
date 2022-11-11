# Regex

### Regular Expressions

{% embed url="https://regexr.com" %}

`[a-c]zz` is the same as above. `azz`, `bzz`, and `czz`.

`[^k]ing` will match `ring`, `sing`, `$ing`, but not `king`.

&#x20;Match any single character (except the line break) is the `.` dot.&#x20;

Set a character as optional in your pattern using the `?` question mark.

That means that `abc?` will match `ab` and `abc`, since the `c` is optional.

`\d` matches a digit, like `9`\
`\D` matches a non-digit, like `A` or `@`\
`\w` matches an alphanumeric character, like `a` or `3`

Underscores `_` are included in the `\w` metacharacter\
`\W` matches a non-alphanumeric character, like `!` or `#`\
`\s` matches a whitespace character (spaces, tabs, and line breaks)\
`\S` matches everything else (alphanumeric characters and symbols)



`{12}` - **exactly 12** times.\
`{1,5}` - **1 to 5** times.\
`{2,}` - **2 or more** times.\
`*` - **0 or more** times.\
`+` - **1 or more** times.

`^` - starts with\
`$` - ends with

Define groups by enclosing a pattern in `(`parentheses`)`

"either/or" pattern example, the pattern `during the (day|night)`
