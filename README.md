# Web-Crawler

## High-level approach
	
Procedure of crawling the fakebook:

1. The first thing to solve is that we have to use the given credentials to login to the website. In this case, we first get the login webpage and fetch the required csrftoken and construct a POST request with the crendentials to login.

2. Once we have the session id, we add the fakebook page to the frontier list and call a craw function to start visiting websites in the frontier and look for secret flags.

The program would quit until: all five secret flags for the given username are found, or crawler have visited all related website but could not find the secret flags(logically yes, but technically could never happen).

## Challenge 

1. Although we dont have to worry about this for grading, but we face chanllenge like network latency, server respond with relatively low speed.

## Test

We use the verbose mode to see if there is anything wrong with the program, and we run the program to see if all flags are found correctly.
