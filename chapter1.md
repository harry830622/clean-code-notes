# Comments

The proper use of comments is to compensate the **failure** to express ourselves in code.

---

## Comments do NOT make up for bad code

If you find your code a mess, **clean it** instead of adding comments!

## Explain yourself in code

A piece of code with a comment:

```cpp
// Check if the shape is a square
if (shape.top_edge_.length_ == shape.bottom_edge_.length_ &&
    shape.right_edge_.length_ == shape.left_edge_.length_ &&
    shape.top_edge_.length_ == shape.left_edge_.length_ &&
    shape.top_left_angle_ == 90)
```

Cleaner one without a comment:

```cpp
if (shape.IsRectangle())
```

## Good comments

### Legal comments

Such as copyright or authorship statements.

### Informative comments

### Explanation of intent

Comment on why you write the piece of code in the way you write it instead of just briefing what it does.

### Clarification

Sometimes, there are some external APIs in your code that you cannot alter to make it more experssive. In this case, comment your code to clarify its purpose.

```cpp
// Check if "Pick up Tony at 5 P.M." is in the todo_list
if (todo_list.find("Pick up Tony at 5 P.M.") != todo_list.end())
```



