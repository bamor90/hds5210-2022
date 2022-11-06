# Notes on the Midterm

* _Correctness    (out of 40):_ 40
* _Good Practices (out of 10):_ 9
* _Docs / Testing (out of 10):_ 1

_Details on the grading criteria for the midterm can be found on [Canvas](https://canvas.slu.edu/courses/28045/rubrics/23671)._

Overall, your code works.  However, you wwere missing the required documentation and testing throughout your code.  The instructions state _All functions require docstrings with a description and at least one test case_. None of your functions had docstrings. I subtracted only 9 points for missing that requirement because you did have a couple of comments.


## Step 1
* Nice work handling the possibility that the format might not match what you're looking for. I think this approach is great. It keeps your code from crashing. Keep in mind that it is sometimes better to have code generate an exception, though, if the file format doesn't match what you're expecting.

## Step 2
* No additional comments.

## Step 3
* This code works, but it does not take advantage of your previously written `get_rate()` function. The cleaner approach here would have been not to repeat all the logic to get to the right code, instead just calling `get_rate()` and then doing the adjustments from there. I've subtracted 1 point from _Good Practices_ for this.

## Step 4
* Nice work making sure your output was rounded at the end. I would recommended doing the rounding while you're accumulating the results rather than doing it at the end.
* You returned your results at a list with two items, which is OK, but Python usually returns the results as a _tuple_ instead of a _list_ in a scenario like this.  That's more of a convention than a requirement, though.
* From a readability perspective, I would recommend mapping the items within each row into another variable name. For example: `visit_date = row[6]` or `hospital = row[1]`.