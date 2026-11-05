PART 1: Bug Analysis
Note to self: Refer to Buggy Program Practice Exercise Code 


Error 1: line 3 is missing : after calculate_stats(numbers). It raises a SyntaxError.
              The Fix:    def calculate_stats(numbers):
	Solved myself
Error 2 : line 10 is missing : after if num > average. It raises a SyntaxError.
              The Fix: if num > average:
	Solved myself
Error 3 : if scores is empty and count is 0, this divides by 0 raising a ZeroDivisionError
	The Fix: On line 6  if count == 0:
          return {
             "total": 0,
             "average": 0,
             "above_average": [],
             "above_count": 0
         }
	Needed help from AI
Error 4 : line 20 “70” is text while the other scores are numbers. This raises a TypeError.
	The Fix: remove the “”   scores = [85, 92, 78, 95, 88, 70, 93]
	Used AI then realized I had overlooked it.
Error 5 : line 24 average is treated as a variable. This raises a NameError.
	The Fix: print(f"Average: {result['average']}")
	Used AI to solve this

PART 2: AI evaluation notes
I decided to use the prompts on my grade analyzer project.
“How can I make this code more pythonic?”
1.	I did not understand every line at first but after asking the AI to explain the code it gave me I learned what it was doing.
2.	I decided to implement the changes that the AI suggested because it helped prevent duplicate logic.
3.	The code continued to work after implementing.
“What edge cases am I not handling?”
1.	AI told me that input validation, runtime errors, and my try block being too broad were all my edge cases. All of which made sense.
2.	I decided to implement the changes to make sure all possibilities were handled.
3.	The code continued to work after implementing.
“Are there any security or reliability concerns?”
1.	AI said there were no security concerns but said to add a if__name__==”__main__”: guard and float formatting to maintain reliability.
2.	I implemented the suggestions to my code.
3.	The code continued to work after the changes were made.
