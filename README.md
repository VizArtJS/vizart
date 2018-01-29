# vizart

> It is recommended to use vizart components.

## Usage: Components

1. Install a vizart component:

```
npm install vizart-basic --save
```

2. import and use

```
import 'vizart-basic/dist/vizart-basic.css';
import { Bar } from 'vizart-basic';

const _bar = new Bar(_domId, _opt)....
```

## Usage: vizart
With this approach, all charts are available.

1. Install VizArt in your project
```
npm install vizart --save
```

2. import and use

```
import 'vizart/dist/vizart.css';
import { Bar } from 'vizart';

const _bar = new Bar(_domId, _opt)....
```

## Three steps to use a chart
1. initialize a chart with domId and declarative options
```
let _opt = {
  ...
};
const _chart = new Chord('#chart', _opt)
```
You only need to provide essential options. [Demo](https://vizartjs.github.io/demo.html) is a good place to check essential options for all charts. You may check up Documentation of each component for full option spec so as to control more chart behaviours.

2. Render a chart with data
```
_chart.render(data) // this should be called only once
```
3. Change a chart on the fly
```
let _opt = _chart.options();
_opt.plots.opacityArea = o.4
_chart.options(_opt);

_chart.update();
```



## Resources

* [Demo](https://vizartjs.github.io/demo.html): quick reference with source code
* [Documentation](https://github.com/VizArtJS/vizart/wiki)

## Components
Production ready:
* [vizart-basic](https://github.com/VizArtJS/vizart-basic)
* [vizart-path](https://github.com/VizArtJS/vizart-path)
* [vizart-core](https://github.com/VizArtJS/vizart-core)
* [vizart-hierarchy](https://github.com/VizArtJS/vizart-hierarchy)
* [vizart-geo](https://github.com/VizArtJS/vizart-geo)

## Credits
My work is based on/inspired by other people's works. You can find links and author names of originals works at each sub module's home page
as well as vizart's demo page.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details



