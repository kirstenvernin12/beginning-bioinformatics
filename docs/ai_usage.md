# AI Use Log

# TASK 12.3 Complete Rosalind Problem #3 Conditions and Loops
- Tool/model & version: Gemini version 0.8.5
- What I asked for: First I had to determine which version of Gemini I was using, so I asked Gemini that. Then I was able to start trouble shooting my code. I was able to generate the correct range of numbers, but was unsure how to get the sum of this range, so I provided my orginal code to Gemini and asked it how to do this. I modified my code to calculate the sum, but still got an error. 
- Snippet of prompt(s): "what version of gemini is this?" (this was a bad prompt). "How do I check the version of gemini that I am using" (this prompt provided code that worked);
  Prompts used to solve the problem: "how do I find the sum of all of the numbers in a range." "how do I correct for this error "TypeError: 'int' object is not iterable""
- What I changed before committing: Gemini provided the following code which did not work to get the version - google-generativeai

  import google.generativeai as genai
  for m in genai.list_models():
  if 'generateContent' in m.supported_generation_methods:
    print(m.name)

  Code that did provide the correct version: import google.generativeai as genai
  print(genai.__version__)

  Changed print (sum(numbers)) to total_sum += numbers
                                    print(total_sum)

- How I verified correctness (tests, sample data): I ran this code and it didn't work, so I changed my prompt and this provided the version. I ran this code with the example numbers and got the correct solution of 7500. 


# TASK P15.32 Complete Rosalind Problem #4 Working with Files
- Tool/model & version: Gemini version 0.8.5
- What I asked for: How to count the number of lines in the object (list_of_lines) in order to create an index so that I can only print the even rows
- Snippet of prompt(s): "how do I count the number of lines in an object"; "how do I only print the even lines in a text file"
- What I changed before committing: I added a counter variable "i" and the "enumerate" function
- How I verified correctness (tests, sample data): I ran the code with the sample data given in the problem to make sure I got the correct output as specified.

# TASK P18.2 Complete Rosalind Problem #5 Dictionaries
- Tool/model & version: Gemini version 0.8.5
- What I asked for: To explain the AttributeError
- Snippet of prompt(s): "AttributeError: 'str' object has no attribute 'items' (gave it the error that I got); how do you count if a word occurs in multiple rows and add the number of times it occurs
- What I changed before committing: Added "if else" statement that checks if the word is already in the word_count dictionary or not. Also, learned that you can print two columns of data as shown in the example by sparating the objects with a comma in the print () function. 
- How I verified correctness (tests, sample data): I ran the code with the sample data given in the problem to make sure I got the correct output as specified.


