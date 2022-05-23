# Edit for more Snippets
# My Markdown-parser
### Initial Failure in all 3 Code Snippets
![Image1](L4-1.png)
**My code does not consider special cases being tested in given 3 code snippets, hence failed.** 
### Changes made to pass Snippet 2
![Image2](L4-3.png)
*For case of nested parentheses, I check if opening and closing parenthesis occur to the left and right (respectively) of first occurence of close Paren.
I count the number of times it occurs ( variable repeat ) and add it to closeParen. Thus, now link would be read uptil last occurence of close Parentheses ( if nesting was present).* 
The presence of backslash means to ignore the close Bracket and rather consider the following as link.
For it, I added the if statement before continue statement.
### Run after change
![Image3](L4-2.png)
**This whole change was just 9 lines of code.** 
