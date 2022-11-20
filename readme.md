### Readme?
ignore this repo , its just my personal cheat.

### Register Effect
```js
gsap.registerEffect({
  name: 'someAnimation',
  effect: (targets, config) => {
    return gsap.to(targets, {
      duration: config.duration,
      y: -200,
      scale: 1.4,
      rotation: 360,
    });
    defaults: {
      duration: 2;
    }
  },
});

gsap.effects.someAnimation(volcano, { duration: 2 });
```

### Stager

```js
gsap.to('.btn', {
  duration: 2,
  stager: 0.2,
  x: 'random(-100,100,100)',
});
```

### fromTo

```js
gsap.fromTo(
    cat,
    {
      x: 0,
      y: -400,
      scale: 0.5,
      rotate: 45,
    },
    {
      x: 0,
      y: 0,
      scale: 1,
      ease: 'bounce',
      rotate: 0,
      duration: 4,
      repeat: 2,
      yoyo: true,
    }
  );
```

