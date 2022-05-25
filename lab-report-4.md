# Edit for more Snippets

*Repository to share ( My own):* [Link-Shared](https://github.com/Anujjain2579/markdown-parser.git)

*Repository to review:* [Link-Reviewed](https://github.com/ddn005UCSD/markdown-parser)
### Tests added to both repositories
![Image1](L4-0.png)
### Initial Failure in all 3 Code Snippets - Shared
![Image1](L4-1-Original.png)
### Initial Failure in all 3 Code Snippets - Reviewed
![Image1R](L4-9-RF.png)
**My code does not consider special cases being tested in given 3 code snippets, hence failed.** 
## Snippet 2
Expected Result 
![Image2RS](L4-11.png)
### Failure in reviewed Code
![Image2R](L4-8.png)
### Failure in shared Code
![Image3R](L4-1-2.png)
### Changes made to pass Snippet 2 - Shared
![Image2](L4-3.png)
**This whole change was just 9 lines of code.** 
*For case of nested parentheses, I check if opening and closing parenthesis occur to the left and right (respectively) of first occurence of close Paren.
I count the number of times it occurs ( variable repeat ) and add it to closeParen. Thus, now link would be read uptil last occurence of close Parentheses ( if nesting was present).* 
The presence of backslash means to ignore the close Bracket and rather consider the following as link.
For it, I added the if statement before continue statement.
### Run after change
Passed Snippet 2 Test
![Image3](L4-2.png)
## Snippet 3
Expected Result
![Image3RS](L4-12.png)
### Failure in reviewed Code
![Image3R](L4-9-Crop.png)
### Failure in shared Code
![Image3R](L4-1-3.png)
### Changes made to pass Snippet 3
![Image4](L4-4.png)
**This whole change was just 7 lines of code.** 
*To overcome the long texts, I found the index of new line character \n. Then we break link into 2 parts and merge again leaving \n. For extra spaces, I used trim() method just before adding the string.*
### Run after change
Passed Snippet 3 Test
![Image5](L4-5.png)
## Snippet 1
Expected Result
![Image2R](L4-10.png)
### Failure in reviewed Code
![Image2R](L4-7.png)
### Failure in shared Code
![Image3R](L4-1.png)
**For considering backticks, I need to consider enclosed string as a code block which requires change in bunch of code lines. The following alone will not work (as in above cases) since it fails other tests. The presence of backticks are in both Brackets and Parenetheses which makes it difficult. Another part that is necessary to incorporate is to read backtick as %60 (ASCII code) in 2nd link.**
![Image6](L4-6.png)
