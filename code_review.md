# Code Review

Code Review is a common section that almost everyday happening in engineering life, 
It is a step that directly affects engineers' mood, at this point, we have to do this more carefully.

On the day I became a Software Engineer, I was started learning to this step - Code Review Process, I saw a lot of failure flows, it even happens every single day, it could from a junior team lead, or even a "senior" team lead but with some irrational political culture.

After several years of exploring how to make my team members comfortable while in the code review process, it may help to earn ownership of what they doing for people in the team, to make the team more powerfully, and together.

## Pull Request

# Commit your code
Before submitting the Pull Request, make sure all commits are able and easy to understand, also clearly to people in the team, not an only reviewer.

Good (one commit)
```
1. Implemented Log-in API with JWT token issuing function.
2. [Database] Fixed schema, remove username field.
3. [Database] Changed userId type to UUID.
```

Bad (one commit)
```
- Finish Login function
```

We expect that range of change in each commit can be as small as possible, but in case of complex changes such as front-end component changes, CSS changes, you can try to use this way to describe your commit.

# Pull Request
TODO: How to create a pull request.

As a reviewer, we review several code reviews per day, but what is better to make our code review more understandable to code provider? We need to comment if we see if there is something that can improve, or a expect error happen.

1. Describe your recommendation as clear as possible.
Code: 
```javascript
  const text = '12345'
  const integer = parseInt(text, 10)
```

Good
```
Could we use the function - `Number()` to convert string to an integer? since we only accept integer, it provides a good way to understanding the code you can see the detailed function usage in the link below.

Reference: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number
```

Bad
```
Use `Number()`.
```

Be joyful, friendly with a rational recommendation.