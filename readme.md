# Symantha
## A super simple semantic high level language for rockstar rookies

- IO
  - **display**
    - logs to the console
    - Example: display "Hello World!" => Hello World!
  - **error**
    - logs out an error
    - Example: error "Something went wrong" => ERROR! Something went wrong
  - **openfile**
    - File Stream (tbd)

- Variables
  - **define [variable-name] to be [String | Integer | Boolean]**
    - instantiates a variable __variable-name__ of one out of three Types
  - **define list [variable-name] with: $arg1, $arg2 ... $argn**
    - Instantiates a variable __variable-name__ of Type Array with multiple values ($argn)

- Operators
  - **plus**
    - Adds Numbers to Numbers, Concatenates Strings, or throws error
    - Example: 1 plus 1 => 2 | "Apples" plus " & " plus "Oranges" => Apples & Oranges
  - **minus**
    - Subtracts Numbers from Numbers or throws error
    - Example: 48 minus 6 => 42
  - **multipliedby**
    - Multiplies Numbers or throws error
  - **dividedby**
    - Divides the first Number from the second Number supplied, or throws error

- Loops and Iterators
  - **incase (condition) do {function} | otherwise (condition) do {function}**
    - If/else statement


### Example
####  helloworld.symt

		intent: "Saying hello to the world"
		special: _ becomes " "

		----

		define greeting to be "Hello"
		define list world with ("Mundo","Welt","World")
    
		make greeter do
		  display greeting plus _ and world(0) plus "!"
		end


#### Console

		STDOUT: Hello Mundo!

