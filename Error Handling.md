# Error Handling

## Introduction
In this section, I will be showing some of the research I have done on error handling in Python for my UW Foundations of Programming course. I utilized articles from [Real Python](https://realpython.com), various YouTube videos, and Chat-GPT for this research. I tried to create engaging and unique examples for my explanation as that usually helps me when learning new concepts.

## Basic Overview of Error Handling
The basic structure of error handling is `try`, `except`, `else`, `finally`. Here is an example image from Real Python (Figure 1).

![Figure 1: Error Handling from author Said van de Klundert at Real Python (External Site)](link to image)

## Example of Error Handling
In my research, I noticed a lot of examples using the errors "divide by zero" and "file not found," so I turned to Chat-GPT for some inspiration for new examples. One of the ideas presented by this LLM was receiving an error for entering a date in the future when using a program that calculates age based on the year born (Figure 2).

![Figure 2: Example of error handling from Chat-GPT](link_to_image)

Here is the full script after I customized and edited what was suggested by Chat-GPT. I added a playful error handling message and the `else`,`finally` clause (Figure 3).

![Figure 3: Customized the script and added “else” and “finally” messages](link_to_image)

## Outputs from Example Script
Let’s see what happens when we run this code with different inputs.
Here we can see the calculation performs correctly with no errors (Figure 4).

![Figure 4: Testing a regular date of 1950](link_to_image)

Here we can see the first exception handled by this script (Figure 5). The year entered is in the future, which is not possible (or is it…?)

![Figure 5: The year entered was a future date, error handled](link_to_image)

Error handling tries to deal with the unexpected, and here is a great example. The first time I tested this script, I entered my full birthday without thinking about it, and of course, an error occurred. This is how the `except` statement handled this (Figure 6).

![Figure 6: A full birthday was entered rather than a year, error handled](link_to_image)

Now let’s look at the output from `else` and `finally`. I noticed other authors used the print statement to explain what the script is doing, and I found that very helpful. Take a look (Figure 7).

![Figure 7: Output from else and finally](link_to_image)

## Summary
The statements `try`, `except`, `else`, and `finally` handle errors that can occur when running a script. The principle is to first try to handle the most specific exception first, then have a general catch-all for any others. Error handling is an approach to making your script work through issues that come up, rather than the entire script stopping and providing information that may not be useful to the user.

Here are some more resources:
- [Geeks For Geeks](link_to_site)
- [Python Exception Hierarchy](link_to_site)
- [Tech World With Nana](link_to_site)
- [Socratica](link_to_site)
- [Corey Schafer](link_to_site)
- [Neural Nine](link_to_site)
- [Arjan Codes](link_to_site)
