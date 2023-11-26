### Warning: This primarily focuses on Luau, this uses OpenAI's ChatGPT for fixing mistakes. 

# How To Luau
Welcome to my Luau Guide! If you're wondering about Lua, here's a quick overview: Luau is a compact programming language designed for applications, games, and engines. It's especially handy in platforms like ROBLOX, where users can harness Luau to create games within the engine.

## Why use Luau
People use Luau for programming in ROBLOX because it's the scripting language specifically designed for the platform, making it easier to create games and interactive experiences within the ROBLOX game environment.

# Let's Start!
We won't go in depth how to install Luau as that should be already easy by going to the `GitHub > Releases > Latest Version > Files`, so we're just going to teach you some basics from the start.

### Variables:
Variables are like words which are stored in your brain, They're crucial for holding data that your program can use!<br/>We will show how to use variables below:

* **Declaration:** We can create a variable, you declare it by giving it a name or also known as an Index. Here's an Example:

```lua
local ExampleDeclaration1
g_ExampleDeclaration = ""
```

* **Assigning Values**: We can also assign a value to these Declarations such as Statements, Numbers and Strings. Here's an Example:

```lua
local ExampleDeclaration1 = true
local ExampleDeclaration2 = 123
local ExampleDeclaration3 = "Hello, World!"
g_ExampleDeclaration = "This is a Global"
```

> Note: You can also set a Variable to `nil` as a placeholder, but it's always better to initialize with the correct value!

There isn't much to say about Variables so we'll continue to Statements :D

### Statements:
Statements is like some of your brain functions, for example the `if` statement would decide if you will speak or not. If it you will you'll open your mouth but if you don't then it'll stay shut! (not a very good example lol)

* Here is the `if`, `else`, `elseif` and `end` statements in use!

```lua
local temperature = 25

if temperature > 30 then
    print("It's hot!")
elseif temperature > 20 then
    print("It's warm.")
else
    print("It's cool.")
end
```

* Here is the `while` statement as well!

```lua
local count = 1

while count <= 5 do
    print("Count: " .. count)
    count = count + 1
end
```

* and also this is the `for` statement

```lua
for i = 1, 5 do
    print("Iteration: " .. i)
end
```

* and at last, the `repeat` and `until` statements :o

```lua
local attempts = 0

repeat
    print("Trying...")
    attempts = attempts + 1
until attempts >= 3
```

* Just kidding this is the last Statement, the `break` and `continue` statements!

```lua
for i = 1, 10 do
    if i == 5 then
        break -- exit the loop when i is 5
    end
    
    print(i)
end
```

These statements are important for your Luau scripts, they allow you to make decisions, repeat actions, and control the execution of your code while also keeping it minimal and small!

### Input & Output:
We will learn about the I/O for Luau, this isn't difficult and should be pretty easy, for output it should use the function called `print`!

Here is a simple example:
```lua
local Example = "Hello, World!"
print(Example)
```

As you can see it's very simple and easy to read, what happens in `print` it'll Output some text into a Console, `print`'s arguments can continue forever as it's a `...`,  this means it can be something like this:

```lua
print("Hello, ", "World!")
```

We will also show `io.read`, just note I have no clue if this is in ROBLOX natively or even Luau natively, but I do know that it's in Lua 5.X.

Here is a example for Input:
```lua
print("Enter your username:")
local Username = io.read()

print("Hello, " .. Username .. "!")
```

`io.read` basically awaits for some input in a Console, it should return a string by default but you can actually convert it to a number by using the function `tonumber(...)` :)

## This is the end for now :(
See ya later, hopefully this was easy to read, please give some recommendations on what I should do next, thank you for reading this!
