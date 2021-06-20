## Animations

- takes vals
  - here _keyframes_ can be used to abstract the some animation details behind a friendly word

## Propteries and Values

- animation-name
  - the name of a keyframe
- animation-duration
  - how long the animation takes
- animation-delay
  - how long to wait before the animation starts
- animation-iteration-count
  - number of times the animation happens
- animation-direction
  - forward, backward, or alternate "cycles"
- animation-timing-function
  - the...speed curve of the animation
- animation-fill-mode
  - styles for an animated element before/after the animation happens
- animation

## An Example

```css
.black-to-white {
  /* 
    b-to-w is the keyframe 
    2s is the duration
    linear is the "speed curve"
    1 is the number of times the thing should happen
  */

  animation: b-to-w 2s linear 1;
}

@keyframes b-to-w {
  0% {
    background-color: #000;
  }
  100% {
    background-color: #fff;
  }
}
```

## A Compound Example

```css
.black-to-white-to-red {
  animation: b-to-w 1s linear 1, b-to-r 2s ease-out infinite 2s;
}
```

## Steps

- a timing fn
- splits a block of keyframes into X-STEPS equal sections
- jumps between the keyframes
- can be useful with sprites
