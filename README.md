# Elixir Enum.each and Process.exit

This example demonstrates an uncommon error that can occur when using `Process.exit` within an `Enum.each` loop in Elixir.  Improper use of `Process.exit` inside `Enum.each` can cause the loop to terminate prematurely and potentially lead to resource leaks or other issues. 

The `bug.ex` file shows the problematic code, where the process exits when the number 3 is encountered. The `bugSolution.ex` demonstrates a more robust approach.  It's crucial to handle potential exceptions or termination signals gracefully to maintain application stability.