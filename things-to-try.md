We saw that IEx lets you use the TAB key to get a list of
possible completions as you are typing:

    iex> Enum.ma⭢
    map/2                map_every/3          map_intersperse/3    
    map_join/2           map_join/3           map_reduce/3         
    max/3                max_by/2             max_by/4

We also saw the `h` function gets help on a module or function:

    iex> h Enum.map
                              def map(enumerable, fun)                           

      @spec map(t(), (element() -> any())) :: list()

    Returns a list where each element is the result of invoking fun on each
    corresponding element of enumerable.

    For maps, the function expects a key-value tuple.

    ## Examples

        iex> Enum.map([1, 2, 3], fn x -> x * 2 end)
        [2, 4, 6]
        
        iex> Enum.map([a: 1, b: 2], fn {k, v} -> {k, -v} end)
        [a: -1, b: -2]

So, find the functions that:

* convert a string to upper case
* returns the length of a string
* can divide a string containing comma separated items into a list of those
  items (so "cat,dog,emu" would become ["cat", "dog", "emu"])
* finds the maximum value in a collection
* joins a list of strings into a single string

Then write an expression that takes the string "cat,dog,emu" and returns
a string where each of the terms is capitalized ("Cat,Dog,Emu")

