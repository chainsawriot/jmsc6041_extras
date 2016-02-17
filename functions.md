# Functions, Subsitution model and scope
By Chung-hong Chan (@chainsawriot)

## Functions: in a non-computer context

The highest point of Victoria Peak is 552 metres. What is highest point of Victoria Peak in feet?

You may know 1 metres = 3.281 feet. Therefore, 552 metres can be converted into feet by:

```
552 * 3.281 = 1811.11
```

Another way to represent the same idea is to create a function, suppose we define a function called `f(x)`

```
f(x) = x * 3.281
```

`f` is the name of the function and `x` is the *argument* of that function. `x * 3.281` is the body of that function. Merely defining a function will not give you the answer, you need to put such function into use to get the answer.

```
f(x = 552) = ?
```

How can we arrive at the answer? we can derive the answer using the *subsitution model*. In this example, when the argument x is 552, we can subsitute the value of x in the function body with 552.

```
f(x = 552) = 552 * 3.281 = 1811.11
```

Excercise 1: The highest point of Tai Mo Shan is 957 metres. Convert it to feet using f(x) by subsitution.

Similarly, you can define more functions for unit conversion, e.g.

Celcius to Fahrenheit, `g(c)`

```
g(c) = c * (9/5) + 32
```

Currency conversion: from Hong Kong Dollar to Euro, `h(hkd)`

```
h(hkd) = hkd * 0.11533
```

And it is not only about mathematics. You can define a function to find out the capital city of a country, `i(country)`

```
i(country) = Google for country + "capital"
```

### A project: Area calculation

The area of a square can be calculate with a function like this:

```
square(side_length) = side_length * side_length
```

This function can be defined in R as such:

```{r}
square_area <- function(side_length) {
  return(side_length * side_length)
}
```

