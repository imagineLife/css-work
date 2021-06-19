## Transitions

**transition**  
The transition describes how a specific css property value _will change_ with a different value.

- Transitions are good for a **single instance**, where an animation happens 1x
- Transitions are good for **granularity**, where fine-tuned effects can happen on hand-picked properties

```css
transition: color 2s;
```

**transition-property**  
_the_ prop that the transition is on.  
https://www.w3.org/TR/2018/WD-css-transitions-1-20181011/

**transition-duration**  
how long the transition takes, in ms

**transition-timing-function**  
some..."room"... this defaults to "ease"

**transition-delay**  
how long before the transition starts

```css
transition: color 2s 150ms;
```

- property: color
- duration: 2s
- delay: 150ms

## On Duration

"_However long your pre-production animation, halve its duration... then halve it again._" - Studio animation rule of thumb

## On Easing

an animation's "rate of change" over time
**see resources** - [Easings.net](https://easings.net/)

### Timing Function Vals

- Linear
- ease-in
- ease-out
- ease-in-out

### A cubic-bezier transition

```css
transition: transform 0.35s cubic-bezier(0, 0.04, 0.98.34);
```
