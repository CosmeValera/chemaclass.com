+++
title = "Clean Code"
description = "A Handbook of Agile Software Craftsmanship"
[taxonomies]
tags = [ "book", "software", "clean-code" ]
[extra]
pages = "460"
author = "Robert C. Martin"
static_thumbnail = "https://images-na.ssl-images-amazon.com/images/I/41yafGMO+rL._SX376_BO1,204,203,200_.jpg"
+++

<a target="_blank" href="https://www.amazon.de/gp/product/0132350882/ref=as_li_tl?ie=UTF8&camp=1638&creative=6742&creativeASIN=0132350882&linkCode=as2&tag=chemaclass-21&linkId=69e7ad0e2974e7511a92cce2c6a08ef0">
    <img border="0" src="https://images-na.ssl-images-amazon.com/images/I/41yafGMO+rL._SX376_BO1,204,203,200_.jpg" >
</a>

<!-- more -->

Even bad code can function. But if code isn’t clean, it can bring a development organization to its knees. Every year,
countless hours and significant resources are lost because of poorly written code. But it doesn’t have to be that way.

### What Is Clean Code?

- The code can be measured with either "good" or "bad" in the code review or by how many minutes it takes you to talk
  about it.
- A clean code should be elegant, efficient, readable, simple, without duplications, and well-written.
- You should add value to the business with your code.
- Clean code offers quality and understanding when we open a class.
- It is necessary that your code is clean and readable for anyone to find and easily understand. Avoid wasting others'
  time.

### Meaningful Names

- Names of the classes, variables, and methods must be meaningful and clearly indicate what a method does or what an
  attribute is.
- Create pronounceable names to facilitate communication.
- Avoid acronyms and avoid confusing names, which may bring anyone who reads the code to the wrong conclusions.
- Use names that reflect the system domain, the context, and the problems that must be solved.

### Functions

- The method should be easy to read and understand.
- The method should convey its intention.
- The methods should be small. Another rule for small methods is that they should be even lower.
- They must have up to 20 lines. (I think they should have up to 10 lines.)
- Methods should only do one thing: they should do it the right way and just do it.
- You should use names with words that say what it really does.
- The optimal number of parameters of a method is zero, after one and two.
- Three should be avoided, but if you think it should be used, have a good justification.
- Parameters of the Boolean type as a parameter already clearly states that it does more than one thing.
- Methods must do something and return something.
- Avoid duplication.

### Comments

- One of the most common reasons for the comments is because the code is bad.
- If you're thinking about writing a comment, then the code should be refactored.
- Comments do not save a bad code.
- Try to explain what the code causes to happen.
- Comments can be useful when placed in certain places.
- Create method names and informative variables instead of explaining the code with comments.
- Comments can be used to express the importance of certain points in the code.
- The best comment is one that needs to be written because your code already explained.
- Do not write comments with redundant, useless, or false information.
- They should not be used to indicate who changed or why, for that already exists in versioning.
- Don’t comment code that will not be used, remove, it just pollutes the code and leaves no doubt in anyone reading.

#### Formatting

- Formatting should indicate things of importance since it is a developer of communication form.
- A messy code is hard to read.
- The readability of the code will take effect on all of the changes that will be made.
- Try to write a class with a maximum of 500 lines. Smaller classes are easier to understand.
- Set a limit of characters per line of code.
- A good character limit on a line is 120.
- Try to keep more next related concepts vertically to create a code stream.
- Use spaces between operators, parameters, and commas.

### Objects and Data Structure

- Follow the Law of Demeter, which says that one M method of an object O can only consume services of the following
  types of objects:
    - The object itself, O.
    - The M parameters.
    - Any object created or instantiated by M.
    - Direct components of O.
    - Make good abstraction and encapsulation.
- Do not make dumb objects.
- Objects hide the data abstraction and expose methods that operate the data.
- Data structures expose your data and do not have significant methods.

### Error Handling

- Error handling should be planned carefully by all programmers.
- When wrong things occur, we have to get it to do the right things.
- We should give preference to launching an exception than treating it just to hide.
- Create messages with information about the error.
- Mention that it failed. Where was this failure? If possible, mention why it failed.
- Look at separate business rules for errors and error handling.
- Avoid returning a NULL in methods, preferably to return an empty object.
- Avoid passing NULL to the methods; this can generate NullPointerExceptions.

### Boundary

- In third-party code, to avoid passing objects, APIs look forward in order to keep things in the same class.
- Perform tests on the API's third party.
- Study the documentation and test the third API before you start using it.
- Check well the features you will use.
- These steps can help increase yield when there are new updates to the API and you can only run your tests to check for
  this update.
- Create tests the functionality of the API.

### Unit Tests

- Make sure each piece of code is doing what you expect it to do.
- Follow the TDDs law:
    - Don't create code before you have a failing test.
    - Don't create more tests than necessary to fail.
    - You cannot write more code than enough to pass the test that is failing.
- Keep your test clean.
- The tests must undergo changes in the same way that the code.
- The dirtier the code, the more difficult test will be to maintain.
- Use the F.I.R.S.T rule for testing:
    - The test is fast-running.
    - The tests are independent of other.
    - The test is repeatable in various environments.
    - The test is self-validating.
    - The test is timely.
- The test is as important as the production code.

### Classes

- By default, classes should start with the variables:
    - Static and constantly public.
    - Static and variable private.
    - Instances and variables privates.
    - Soon after comes the functions.
    - The class name should represent your responsibility.
- The class must have only one responsibility.
- To know the size of the class is ideal, or we should not measure her responsibility.
- You should try to make a brief description of the class.
- The methods should be:
    - Small...
    - ...and even lower.
- They must have only one responsibility.