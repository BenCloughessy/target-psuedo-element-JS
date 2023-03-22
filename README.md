# Targeting Psuedo-Elements with Javascript

It typically makes more sense to work with your DOM than try to target a css psuedo-element specifically. That said, I have been in professional situations where altering the DOM
adds significant complexity. For small problems, I've found this to be a wonderful solution.

# Pointer Events
We can control whether or not an element responds to pointer events, such as a click event. Further, we can distinguish between the psuedo-element and the rest of the element.
By setting pointer-events:none for a container, and then pointer-events:all for a psuedo, we effectively target the psuedo-element even though our JS is targeting the whole element.
It has significant limitations, but in certain contexts in can be helpful.
