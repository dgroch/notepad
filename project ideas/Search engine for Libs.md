# What is it?

Search engine / graph that helps developers find the best libs

# How it works (Elixir)

Given user is on the home page
Then user can see a list of concerns (eg authentication)
When the user clicks a concern
Then the user is taken to the list of concerns page
And the user can see a list of lib descriptions ranked by popularity

Given the user is on the home page
When the user enters search information
Then the user is taken to the list of concerns page 
And the user can see a list of lib descriptions ranked by popularity

Given the user is on the list of concerns page
When the user clicks on a lib description
Then the user is taken to the lib detail page

Given the user is on the lib detail page
Then the user can list a list of similar libs ranked by popularity 

# Implementation

## Authority

1. Find all the Elixir projects on Github
2. Get the deps page foreach project
3. Iterate each page and estimate [page rank](http://www.cs.princeton.edu/~chazelle/courses/BIB/pagerank.htm)

## Similarity

1. Find all the Elixir projects on Github
2. Get the title / descriptions from each README
4. Reduce corpus to verb / adjectives
5. Count the words 
5. Extract features via TFIDF
6. Create a nearest neighbour model
7. Deploy as web service

# Questions

Is there a taxonomy of CS concerns that could be used?