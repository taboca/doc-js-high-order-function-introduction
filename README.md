# Introduction to High Order Functions

* Ref https://www.youtube.com/watch?v=BMUiFMZr7vk - the following is a parallel annotation to the class given by Mr. above, Spotify developer.

*Create an anonymous function and assign it to a variable* is common in functional programming languages. Just like strings, or numbers, functions can be assigned to variables.

```
var multiply = function(x,y) {
   return x*y;
}
```

Take one function and put it inside another. This other, that receives a function, is referred as High Order Functions. With that, you can enable composition, to put small functions inside other functions.

On the other hand, the function that you put within other functions are referred as callback functions.

```
var cities = [
   { name: 'Boston', state: 'Massachusetts', country: 'United States' },
   { name: 'Ribeirao', state: 'Sao Paulo', country: 'Brazil'},
   { name: 'Sao Carlos', state: 'Sao Paulo', country: 'Brazil'},
]

var brazilianCities = cities.filter(function(city) {
   return city.country === 'Brazil;
});
```

Therefore, as "filter" in the Array accepts a function, then filter is then a referred as a High Order Function.
