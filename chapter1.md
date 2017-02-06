# Comments

The proper use of comments is to compensate the **failure** to express ourselves in code.

---

Comments can lie. The older they are, the more likely they are wrong. Because we just cannot maintain them while improving and updating our code.

## Comments do NOT make up for bad code

If you find your code a mess, **clean it** instead of adding comments!

## Explain yourself in code

A piece of code with a comment:

```cpp
// Check if the rectangle is a square.
if (rectangle.TopEdgeLength() == rectangle.LeftEdgeLength())
```

Cleaner one without a comment:

```cpp
if (rectangle.IsSquare())
```

## Good comments

### Legal comments

Such as copyright or authorship statements.

### Informative comments

Provide basic information.

> It's the least desirable form IMO.

### Explanation of intent

Comment on why you write the piece of code in the way you write it instead of just briefing what it does.

### Clarification

Sometimes, there are some external APIs in your code that you cannot alter to make it more experssive. In this case, comment your code to clarify its purpose.

```cpp
// Check if "Pick up Tony at 5 P.M." is in the todo_list.
if (todo_list.find("Pick up Tony at 5 P.M.") != todo_list.end())
```

### Warning of consequences

For example, warn others if a function might spend too much time or even run out of memory.

### TODO comments

They are like reminders. Just remember to check them regularly to eliminate the completed ones.

### Amplification

Emphasize the detail that might seems not important.

```js
function addUser(userName) {
  // userName must be trimmed to avoid invalid names such as '   '.
  if (userName.trim().length !== 0) {
    // do something...
  }
}
```

### Public APIs



