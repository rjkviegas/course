# Thermostat: saving state

[Back to the Challenge Map](README.md)

There is an issue with your thermometer interface!  If you close your browser and reopen it, it forgets what settings you had. It has no persistence. Over the last couple of weeks how have we managed persistence in our applications?

* Create a remote API that the thermostat can talk to. (hint: you can build your own web server to provide this API using Sinatra!).
* Update your UI so that the thermostat communicates changes to the API. For example, it could make a POST request to localhost:4567/temperature, with the new temperature.  On page refresh, the thermostat could make a GET request to localhost:4567/temperature to get the temperature.
* Save the selected city information using the API too.

## Resources

There is an example of how to approach this challenge [here](https://github.com/soph-g/thermostat-exemplar). Read the README carefully before looking through the code, there are several branches showing different solution options.

## Walkthrough

You'll be able to use a lot of the same techniques as the ones you used in week 4. Consider having a look at those walkthroughs if you get stuck.

![Tracking pixel](https://githubanalytics.herokuapp.com/course/thermostat/saving_state.md)
