### Elixir - Parallel Weather App

#### How to use it

- $ cd app
- $ mix test
- $ mix deps.get
- $ iex -S mix

``` ruby

// spawn version
iex> cities = ["Rio de Janeiro", "Niteroi", "Sao Paulo", "Porto Alegre"]
["Rio de Janeiro", "Niteroi", "Sao Paulo", "Porto Alegre"]

iex> App.Weather.start cities
[{#PID<0.176.0>, "Rio de Janeiro"}, {#PID<0.176.0>, "Niteroi"},
 {#PID<0.176.0>, "Sao Paulo"}, {#PID<0.176.0>, "Porto Alegre"}]
Niteroi: 32.7 °C, Porto Alegre: 20.8 °C, Rio de Janeiro: 32.7 °C, Sao Paulo: 30.8 °C

// task version
iex> cities = ["Rio de Janeiro", "Niteroi", "Sao Paulo", "Porto Alegre"]
["Rio de Janeiro", "Niteroi", "Sao Paulo", "Porto Alegre"]

iex> App.SimpleWeather.start cities
["Rio de Janeiro: 30.3 °C", "Niteroi: 30.3 °C", "Sao Paulo: 28.0 °C",
 "Porto Alegre: 25.8 °C"]
```

``` ruby
Compiling 1 file (.ex)
....

Finished in 0.9 seconds
4 tests, 0 failures

Randomized with seed 217833
```

#### Enjoy!
