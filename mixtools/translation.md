# Translation guide 
You can learn how to translate mixtools message.  
Please note that do not delete any variables in the message text, as variables can only be moved.  
### Example 1:
```
Economy:
  Balance: "&aYour money: &e%1$s %2$s"
```

This is the balance message text in economy.  
MixTools uses `String.format(String s, Object... args)` to replace variables,  
so `%1$s` is the currency symbol(can set in config or command) and `%2$s` is the player's balance.