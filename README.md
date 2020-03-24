# interp1

[MATLAB-inspired](https://www.mathworks.com/help/matlab/ref/interp1.html) 1-dimensional data interpolation.

## Import

You can import the function using.

```javascript
import interp1 from 'interp1'
```

## API

```javascript
vqs = interp1(xs, vs, xqs);
vqs = interp1(xs, vs, xqs, method);
```

The function takes the following arguments:

- `xs`: Array of independent sample points. No value may occur more than once.
- `vs`: Array of dependent values v(x) with length equal to xs.
- `xqs`: Array of query points.
- `method`: Method of interpolation: `linear`, `nearest`, `next` or `previous`. Defaults to `linear`.

It returns an array of interpolated values `vqs`, corresponding to the query values `xqs`.

## NPM scripts

- `npm install`: Install dependencies
- `npm test`: Run test suite
- `npm start`: Run `npm run build` in watch mode
- `npm run test:watch`: Run test suite in [interactive watch mode](http://facebook.github.io/jest/docs/cli.html#watch)
- `npm run test:prod`: Run linting and generate coverage
- `npm run build`: Generate bundles and typings, create docs
- `npm run lint`: Lints code
