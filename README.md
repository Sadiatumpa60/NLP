# What is Natural Language Processing?
Natural language processing is a massive field of study and actively used practice which aims to make sense of language using statistics and computers. In this course, you will learn some of the basics of NLP which will help you move from simple to more difficult and advanced topics. Even though this is the first course, you will still get some exposure to the challenges of the field such as topic identification and text classification. Some interesting NLP areas you might have heard about are: topic identification, chatbots, text classification, translation, sentiment analysis. There are also many more! You will learn the fundamentals of some of these topics as we move through the course.

## What exactly are regular expressions?

Regular expressions are strings you can use that have a special syntax, which allows you to match patterns and find other strings. A pattern is a series of letters or symbols which can map to an actual text or words or punctuation. You can use regular expressions to do things like find links in a webpage, parse email addresses and remove unwanted strings or characters. Regular expressions are often referred to as regex and can be used easily with python via the `re` library. Here we have a simple import of the library. We can match a substring by using the re.match method which matches a pattern with a string. It takes the pattern as the first argument, the string as the second and returns a match object, here we see it matched exactly what we expected: abc. We can also use special patterns that regex understands, like the \w+ which will match a word. We can see here via the match object representation that it has matched the first word it found -- hi.

## Common regex patterns

There are hundreds of characters and patterns you can learn and memorize with regular expressions, but to get started, I want to share a few common patterns. The first pattern \w we already saw, it is used to match words. The \d pattern allows us to match digits, which can be useful when you need to find them and separate them in a string. The \s pattern matches spaces, the period is a wildcard character. The wildcard will match ANY letter or symbol. The + and * characters allow things to become greedy, grabbing repeats of single letters or whole patterns. For example to match a full word rather than one character, we need to add the + symbol after the \w. Using these character classes as capital letters negates them so the \S matches anything that is not a space. You can also create a group of characters you want by putting them inside square brackets, like our lowercase group.

## Python's re module

In the following exercises, you'll use the `re` module to perform some simple activities, like splitting on a pattern or finding all patterns in a string. In addition to split and findall, search and match are also quite popular. You saw a simple match at the beginning of this video, and search is similar but doesn't require you to match the pattern from the beginning of the string. The syntax for the regex library is always to pass the pattern first, and the string second. Depending on the method, it may return an iterator, a new string or a match object. Here we see the re.split method will take a pattern for spaces and a string with some spaces and return a list object with the results of splitting on spaces. This can be used for tokenization, so you can preprocess text using regex while doing natural language processing.

























# NLP Dataset - https://www.kaggle.com/datasets/basilb2s/language-detection
