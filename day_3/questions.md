## Day 3 Questions

1. What is a conditional statement? Give three examples.
* A conditional statement takes certain code and processes them as true and false to determine its output.
  * if minutes < 7
    puts "The water is not boiling yet."
  * elsif minutes == 7
    puts "It's just barely boiling"
  * elsif minutes == 8
    puts "It's boiling!"
  * else
    puts "Hot! Hot! Hot!"
    * This gives us multiple conditions. If the value of minutes is less than 7, equal to 7, equal to 8, or more than 8, we will have different results.

1. Why might you want to use an if-statement?
If you are receiving input from a user and need multiple outcome choices from what their response is.

1. What is the Ruby syntax for an if statement?
if conditional [then]
   code...
[elsif conditional [then]
   code...]...
[else
   code...]
end

1. How do you add multiple conditions to an if statement?
By using elsif and else.

1. Provide an example of the Ruby syntax for an if/elsif/else statement:

puts "A wizard offers you three concotions and promises immortality if you choose the right one"
puts "1. A drink labeled 'Live Forever'"
puts "2. A drink labeled 'It's this one, I promise'"
puts "3. A drink labeled 'Don't drink this'"

print "> "
drink = $stdin.gets.chomp

if drink == "1"
  puts "You feel the power of immortality take over you."

elsif drink == "2"
  puts "You start to feel your throat clench."
  puts "1. This is just the beginning of the transformation. Wait until it takes full effect."
  puts "2. Reach for the drink labeled 'Live Forever'."
  puts "3. Reach for the drink labeled 'Don't drink this'."

  print "> "
  drink2 = $stdin.gets.chomp

  if drink2 == "1"
    puts "You can't breathe and don't have the strength to reach for another drink anymore. You die."
  elsif drink2 == "2"
    puts "You grab the drink just in time. You are now immortal."
  elsif drink2 == "3"
    puts "Why would you drink this with that label? You die instantly."
  end

elsif drink == "3"
  puts "You've made a grave mistake. It said 'Don't drink this'! You die instantly."

else
  puts "You don't need this drink. You decline and the wizard informs you that you will die in 32 years surrounded by loved ones."
end

1. Other than an if-statement, can you think of any other ways we might want to use a conditional statement?
For numerical values
