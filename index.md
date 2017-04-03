## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/rtlayzell/rush-www/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

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

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/rtlayzell/rush-www/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
