# **Instructions**

Maxlifetime is set to a high number to disable it because the buttons to toggle mutation breaks it, also i don't know if it's a good feature in this case.

The current default settings are cells arranged as a glider in B23/S23 and mutationRate: 0.1.

You can change mutationRate, reproduceCount(birth rules) and survival rules(at line 189), and mutationRate.

You can also draw but it draws the last created cell.

I recommend disabling mutation a bit before it seems good because cells compete a bit after you disable it before mostly stabelizing.


# **How it works**

This evolutionary cellular automata works by randomly selecting one of the parent cells that made the cell, and the offspring inherits its rules with a chance of mutating it by 1 value.

The colors is determined after the birth rules, the lighter it is the higher the rule value is. (I don't know exactly how it works.)


# **Bugs and other issues** 

Disabling mutation disables the lifetime as well. Setting the lifetime to -1 really breaks it.

Can't mutate survive survival rules, rule value is only reproduceCount.

Drawing draws random cells instead of the initial rule.

Spaceships don't emerge.



# **More features to possibly add**

A check to see if mutation is on.

A way to check the cells rule.

Random age.

Add mutation type where it can mutate to a random rule in addition to changing by 1 value.

Mutating groups of cells instead of each cell individually.

Generation count.

Diversity(amount of rules).

Total population.

Pause while drawing.

Add additional drawing algorithm that can be turned on that draws in the most populous rule.

Toggle to make still lives not die from lifetime.

Options to start grid with random cells and rules.

UI

Pause and resume, restart, next step, save and load cell configuration and parameters.

Non-totalistic rules, multiple states, larger than life, non-totalistic rules.

Non-deterministic rules.

Food and predation.


# **Open-ended questions**

What causes these large period oscillators to emerge?

Why do spaceships not emerge, is this inherent to something in the simulation?

Why do large seemily non-oscillating structures that have a stable size form?

What causes the robustness and self-repairment with some parameters? (To test this set the survival rule to something like neighbors < 1 || neighbors > 8 ), the lifetime to 2, reproductionCount to something like [1,2,8] and mutationRate to 0.01 and wait, lower the mutation rate if it didn't work, if it's too slow make it higher. When the cells are in separete patterns that look like oscillators disrupt the oscillator a bit by drawing, if it worked it should have a high chance of repairing.)
