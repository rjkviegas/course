# Code Review Requests

## When to request a code review

There are two main reasons for requesting a code review while at Makers:

  1. You are seeking feedback on how you can improve your code, or
  2. You are seeking feedback on the code as evidence of achieving a goal

Before requesting a code review think about why you are requesting the review, and how you will use the feedback you receive.

## How to request a code review

**tl;dr**
Use this [form][1] to request a review of your weekend challenge or codebase including your own mini review. A coach will then review and give feedback as notes on the PR or via slack.

---
In order to submit the form the following information is required:

### First & Last Name
So the reviewer knows where to send feedback. Make sure your profile name in GitHub is something that could be used to identify you.

### URL
The link to the Github Pull Request or repository.

### Mini Review
This is by far the most important piece here, and what you should include depends on your reasons for requesting the review.

#### Mini review when requesting feedback to improve the code

- What do you think you did well?
- What did you find difficult?
- What would you like feedback on - be as specific as possible!

**Example**
```
I thought my implementation of RESTful routing and MVC went well.
I found it difficult to know what logic should sit in Model, Controller and View. I also found it hard to write feature tests and unit tests.
I would like feedback on my feature test coverage - have I covered everything I should? Also, I am not sure I have used doubles correctly in my tests, so feedback on this would help me to know whether I am on the right track.
```

#### Mini review when requesting feedback on the code as evidence

Be as specific and detailed as possible!

- What goal(s) do you think this is evidence for achieving?
- Why do you think this is good evidence of achieving the goal(s)?

**Example**
```
I think this code is evidence of being able to test drive anything because:
- I followed a TDD process throughout, even managing to test drive my integration with the BBC News API.
- I have used doubles with dependency injection to successfully isolate unit tests.
- The commits are aligned with my test driving process, so each commit contains a test and the code to pass that test.
```

It can be a paragraph/bullet points in the code review request form; notes in the README; a link to your Diode; or notes on your own PR. The better your review is, the more helpful the code review can be as the reviewer will better understand the feedback that will benefit you.

#### NB: A coach will not review code that hasn't a mini-review by the requester.

If the reviewer isn't sure why you're asking for the review, or what feedback would be useful, it's likely they will ask for clarification before doing the review.

---

As always if you have questions about this process or feedback to share about it, please don't hesitate to slack a coach.

[1]: https://code-review.makersacademy.com/reviews/new

![Tracking pixel](https://githubanalytics.herokuapp.com/course/request_a_code_review.md)
