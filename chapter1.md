# Comments

The proper use of comments is to compensate the **failure** to express ourselves in code.

---

## Comments do NOT make up for bad code

If you find your code a mess, **clean it** instead of adding comments!

## Explain yourself in code

A piece of code with comments:

```cpp
// Check if "Pick up Tony at 5 P.M." is in the todo_list
if (todo_list.find("Pick up Tony at 5 P.M.") != todo_list.end())
```

Cleaner one without comments:

```cpp
if (todo_list.includes("Pick up Tony at 5 P.M."))
```

## Good comments



