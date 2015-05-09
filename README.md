---
  tags: todo, basics, tdd
  languages: ruby
  resources: 2
---

## Intro to TDD, RSpec, and Learn

A lot of labs on Learn include tests that verify that the code you write behaves and produces the desired result. It's a sort of an abstract concept at first, but it's worth starting to understand, not only so you can be more productive on Learn, but also because Test-Driven-Development, TDD, is considered the most reliable methodology for delivering quality code. TDD is practiced by the best developers in the world and ignored at the peril of the rest. We'll introduce it to you slowly and you'll quickly get the heart of it.

### What's a Test?

Often when programming we know what we want our program to do but we aren't sure how to make that happen. Sometimes, we're not even 100% sure that the code we wrote will always behave as we expect.

Imagine needing to write a method, `current_age_for_birth_year`, the purpose is to figure out how old a person currently is based on the year the person was born. A method like this is probably used on the majority of social networks. I tell Facebook that I was born in 1984, the year is currently 2015, Facebook knows that I am currently 31 years old. Next year, without updating Facebook at all, because of this working method, Facebook will know that I'll be 32.

Thinking about the example above, we could define the following requirement of our code.

If the year is currently 2015 and I was born in 1984, when I call the method `current_age_for_birth_year` and provide it my birth year, 1984, by passing that year as an argument, `current_age_for_birth_year(1984)`, I expect it to return 31. 

Expressing that narrative in code is called a test. In an idea world, I could code this requirement with something like:

```
I expect the method current_age_for_birth_year(1984) to return 31
```

 The [RSpec Testing Framework](http://rspec.info/) is a ruby library designed to allow programmers to describe the behavior and outcomes of their programs in a very natural language similar to the above example. Lots of Ruby and Ruby on Rails labs on Learn include RSpec tests. Let's learn a bit about RSpec..

 ### How Does RSpec and Learn Work?

At this point all we want you to be able to do is understand testing at a high level, run tests, read test output, and be familiar, ideally comfortable, with test code.

The first thing you should know is that the `learn` terminal command, installed by the `learn-co` gem, runs the tests included with all labs on Learn. Whenever you want to test your code and see if it's working, simply execute `learn` from within the lab's directory.

The idea is that labs come with expectations for how your code should behave and you write the code to make those tests work.

All of our tests are located within the `spec` directory.








