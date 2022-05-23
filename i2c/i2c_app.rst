I2C
###
Setting up I2C on Raspberry
---------------------------

Install OpenPlotter I2C app
+++++++++++++++++++++++++++
Go into >Openplotter>Settings and then hit refresh.

In the list of openplotter Apps, go down to I2C Sensors and select then install.

Switching on I2C on your Raspberry
++++++++++++++++++++++++++++++++++
In the menu of Raspbian OS, go to >Preferences>Rasp Pi Config to start the Raspberry Config tool.

Select [5 Interfacing Options], and then enable I2C.

Once enabled, hit <Finish> and reboot your Raspberry. After reboot, I2C bus is enabled.

.. image:: https://www.raspberrypi.com/documentation/computers/images/raspi-config.png

Further information can be found on thr official Raspberry website. [1]_

Powerdown the Pi and install the sensor(s)
++++++++++++++++++++++++++++++++++++++++++

I2C uses several pins - pins1 (3.3V), 3(SDA), 5(SCL), 9(GND).  Connect them up accordingly based on your devices.

Power the Pi back up

Got to >Openplotter>I2C and add all sensors providing a name for each that makes sense and fits with the Signal K specification, see http://signalk.org/specification/1.0.4/doc/signalk.pdf, see the picture below:

.. image:: img/i2c1.png

On the connection Tab, add connection to Signal K for each of the sensors:

.. image:: img/i2c2.png

.. note::
	The Pypilot entry will not show up until you have done the Pypilot configs

.. [1] https://www.raspberrypi.com/documentation/computers/configuration.html#raspi-config
