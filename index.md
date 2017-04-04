<span style="font-size: 1.4em">Rush is a General Purpose Programming Lanuage that builds on top of today's most widely used and popular languages.</span>
### Features
- Strongly typed with type-inference.
- Multiparadigm with emphasis on functional techniques.
- A rich feature set for the utmost expressiveness.

```
import std.io
import std.math

struct point:
    x: floating get set;
    y: floating get set;

    this(x, y: floating):
        this.x = x;
        this.y = y;

tostr({x, y}: @point) => $"({x}, {y})";

main(args: string[]):
    let step = pi / 5;

    let xs = map(1...10, x => cos(x * step));
    let ys = map(1...10, y => sin(y * step));

    let pts = zip(xs, ys).map({x, y} => new point(x, y));

    each(pts, writeln);
```