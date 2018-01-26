# Programming Model


Workflow process.
1. You write a script and execute it against spark.
1. Spark parses the script by:
  1. Consuming the file and turning it into a plan.
  1. Optimizing it.
  1. Executing it.


What this means for you:

When writing spark code NOTHING is evaluated until you call for an action.

Sample actions are:
* dataset.write()
* dataset.collect()
* dataset.show()
* dataset.count()
* etc


Why is this important?
* This kind of programming model can cause quite a bit of confusion, when something breaks at runtime it will always
show the failure initially occurring at the point of breakage.
* There will always be a hint as to where the failure
actually occurred but it's significantly more effort to find.