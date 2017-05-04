##############################################################################################
STM32F4 - Weather Station

Using the Nucleo64-466RE board and the following modules:
AM2320
Tinyrtc/ds3231sn
1.4inch SPI LCD TFT (ST7735)
ONE Wire Temp

The code will read the temperature and humdity from AM2320 and the temperature from the one wire temp module,
and with the time from the ds3231sn send the data via serial using csv.
The information will be shown on the st7735 lcd with 5mins interval of temperature and a real time clock with date.

The data will be received via python than using blaze/panadas the data will be placed into a dataframe to be stored into mongodb.
Python will process the data having MIN, MAX , AVG temperature of the day, month with their respective time log.
Python will have graphs for the MIN,MAX,AVG of yesterdat , today, but also have a streaming graph for the current temperature.
The information can be view via GUI or WEB using flask.

Graphing python modules:
Matplotlib
Bokeh
Gadfly
Plotly

Framework:
Flask
#################################################################################################################

