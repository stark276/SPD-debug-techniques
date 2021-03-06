# Debug Log

**Explain how you used the the techniques covered (Trace Forward, Trace Backward, Divide & Conquer) to uncover the bugs in each exercise. Be specific!**

In your explanations, you may want to answer:

- What is the expected vs. actual output?
- If there is a stack trace, what useful information does it contain?
- Which technique did you use, on which line numbers?
- What assumptions did you have about each line of code, and which ones were proven to be wrong?

_Example: I noticed that the program should show pizza orders once a new order is made, and that it wasn't showing any. So, I used the trace forward technique starting on line 13. I discovered the bug on line 27 was caused by a typo of 'pzza' instead of 'pizza'._

_Then I noticed another bug ..._

## Exercise 1

[["TypeError: 'topping' is an invalid keyword argument for PizzaTopping" where the variable access is incorrectly.
-- On line 84 it says "werkzeug.routing.BuildError: Could not build url for endpoint '/'.
 I have changed the redirect from `redirect(url_for('/'))` to `redirect('/')`
]]

## Exercise 2

[[The output was the temperate at the city submitted but the output is an API error. An Internal Server Error is thrown with a backend message of "'city': result_json['name'], KeyError: 'name'". This is thrown because something is wrong with the API call.
]]

## Exercise 3


[[Actual output is a list indexing error. The first error I get when running the file is "arr[k] = right_side[i] IndexError: list index out of range". This tells me that a list is being sorted through incorrectly.

I changed arr[k] = right_side[i] to arr[k] = right_side[j]. Another error saying "TypeError: list indices must be integers or slices, not float" came afterwards. I fixed this by wrapping the mid variable as an integer.]]
