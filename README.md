# **Instructions**

Maxlifetime is set to a high number to disable it because the buttons to toggle mutation breaks it, also i don't know if it's a good feature in this case.

The current default settings are cells arranged as a glider in B23/23 and mutationRate: 0.1.

You can change mutationRate, reproduceCount(birth rules) and survival rules(at line 189), and mutationRate.

You can also draw but it draws the last created cell.

I recommend disabling mutation a bit before it seems good.


# **How it works**

This evolutionary cellular automata works by randomly selecting one of the parent cells that made the cell, and the offspring inherits its rules with a chance of mutating it by 1 value.
The colors is determined after the birth rules, the lighter it is the higher the rule value is. (I don't know exactly how it works)


# **Bugs and other issues** 

Disabling mutation disables the lifetime as well. Setting the lifetime to -1 really breaks it.

Can't mutate survive survival rules, rule value is only reproduceCount.

Drawing draws random cells instead of the initial rule.

Spaceships don't emerge.



# **More features to possibly add**

Add a check to see if mutation is on.

Pause while drawing.

Add additional drawing algorithm that can be turned on that draws in the most populous rule.

Toggle to make still lives not die from lifetime.

Options to start grid with random cells and rules.

UI

Pause and resume, restart, next step, save and load cell configuration and parameters.

Multiple states, larger than life, non-totalistic rules.

Non-deterministic rules

Food and predation?
