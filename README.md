![Pipe Architecture](https://d262ilb51hltx0.cloudfront.net/max/1600/1*_zKyCugLRs0pZrq621ZnCg.png)

## Pipe Client Library

### Plottables 

Plottables are ready-to-use, standardized data visualization components. Pipe comes with many built-in Plottables (check them out here: http://pipend.github.io/pipe-web-client/).

Using a Plottable can be as easy as:

```
plot(withOptions(timeseries, {
    x: d => d.time
  , y: d => d.value
})
```

Technically Plottables are composable monads. They’re a lot more fun to use in LiveScript syntax (we will discuss LiveScript use in Pipe in another post).




## Transformation Library
[Repo](https://github.com/Pipend/pipe-transformation)

Transformation module contains utility data manipulation and statistical functions.

These functions are available in Transformation and Presentation blocks in a Pipe query.

To give you a taste of this module:

```
summaryStatistics([Number]) => {mean, sigma, median, length}

fillIntervals(list, defaultValue = 0) => list
```



## Transpilation Library
[Repo](https://github.com/Pipend/transpilation)
