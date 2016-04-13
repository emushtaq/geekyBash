# geekyBash
My repo collecting some silly geeky bash configs

Add the following scripts to your .bashrc/.zshrc or any other bash config 

- Weather

A simple wrapper which picks the city argument and passes it to the super cool wttr API.

```
weather() {
  curl -4 http://wttr.in/"$@"
}
alias -g weather="weather"
```
and when you want to check the weather from your terminal, you just run `weather ******` for example, 
`weather kaiserslautern`
and you get a well formatted weather forecast for the city that you enter in the terminal.

Check out more from the developer of the wttr API [https://github.com/chubin/wttr.in]
