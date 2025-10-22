# Assignment 3 - Write UP

## Description
This assignment completes our movie chatbot system by implementing action functions that query our movie database and building a natural language interface. You implemented functions to search for movies by year, director, and actors, as well as the core search system that matches user queries to appropriate database operations. This builds directly on the pattern matching work from Assignment 2 to create a functional conversational AI system.

## What to complete
1. Complete all action functions in `a3.py` (title_by_year, title_by_year_range, etc.)
2. Implement the `search_pa_list` function to handle pattern matching and responses  
3. Add at least one new movie to the database with proper formatting
4. Create a new pattern/action pair and add it to the pa_list
5. Ensure all provided assert statements pass
6. Complete the reflection questions below
7. Push your code to github for grading

## Reflection Questions

1. What are some key programming concepts or techniques that you learned while completing this assignment?
  
  Some key programming concepts I learned while completing this assignment were tuple structures and how they can be used to store data, and how to import and use outside files in python.

2. How does the overall movie chatbot system work? Explain the flow from when a user types a query to when they receive an answer.

  The chatbot consists of a series of functions, which are called upon when matched with the corresponding pattern of the user’s question. When the user types in their query the program splits the string into a list, which is then passed through search_pa_list. The list of words is now compared to the paired patterns and action function in pa_list; it is then passed through the match function to determine if there is a match between the source and pattern in pa_list. If the match function returns a result (not none) the program sets it equal to the answer and prints it out.

4. What are some real-world applications where this type of pattern-matching chatbot system could be useful? How might you extend or improve this system for practical use?

  This type of pattern-matching chatbot could be used for a FAQ-style of user/customer support, which it already has been used for. To improve this chatbot system you could expand the movie database by pulling from an API, which would make the system more up to date on movies the user would likely ask about.
