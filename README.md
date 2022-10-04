# temperature-sensor
## Temperature, humidity and pressure sensor which you can access through web site.

I have used few sources and compiled together something that works.
It is ongoing projects which uses ESP 8266 in conjuction with BME280. As a starting point I have followed **[this](http://projects.xief.net/?p=638)** instructions.
I'm aiming for low power solution, which includes ESP deep sleep.

How it works:
- ESP is waking up and connecting to WIFI, then it reads sensor and sends the data to my web page and goes back to sleep
- php sctript on my page is inserting received data into database
- When I open web page and want to check values and graph them chart-data php script is querying the database
- then I have used fusioncharts to display values on web page

My page address is: [essencya.pl](https://essencya.pl/) - feel free to check it out, but remember it is still being tested. 
