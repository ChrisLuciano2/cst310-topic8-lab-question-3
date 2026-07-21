# CST-310 · Topic 8 · Lab Question 3

**Question:** Carefully read the description of Project 8. Do you think the use of shaders will simplify the implementation?

Full answer is in
[`Topic 8 Lab Question 3.docx`](./Topic%208%20Lab%20Question%203.docx).

## Summary

Shaders simplify the parts of Project 8 that are inherently per-vertex
or per-fragment math (lighting, height/normal-based coloring, cheap
time-based animation via a uniform) at the cost of upfront plumbing
(compiling/linking two GLSL files and wiring uniforms) that eats into a
100-line C++/OpenGL budget. Net: they simplify the *behavior*, not the
line count, for a scene this small.
