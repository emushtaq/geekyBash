# geekyBash
My repo collecting some silly geeky bash configs

Add the following scripts to your .bashrc/.zshrc or any other bash config 

- Weather

A simple wrapper which picks the city argument and passes it to the super cool wttr API (which internally pokes the WorldWeatherOnline API).

```
weather() {
  curl -4 http://wttr.in/"$@"
}
alias -g weather="weather"
```
and when you want to check the weather from your terminal, you just run `weather ******` for example, 
`weather kaiserslautern` OR just hit `weather` and it will display the weather based on IP. You can pass the following as arguments:

  1. city name
  2. airport code (3 letters) eg: MUC
  3. domain name eg: @stackoverflow.com
  
and you get a well formatted weather forecast for the city that you enter in the terminal.

![Alt text](https://cloud.githubusercontent.com/assets/10843074/14499253/d5cac428-019d-11e6-8c6f-fa7dffe81859.png)

Check out more from the developer of the wttr API [https://github.com/chubin/wttr.in]
