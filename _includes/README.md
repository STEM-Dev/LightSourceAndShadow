LightSourceAndShadow
=========================

NetLogo Model of Light source(s), a movable screen, and a light-sensitive film used for an introductory course on modeling.

![screenshot](https://raw.githubusercontent.com/VicCastillo/LightSourceAndShadow/master/LightSourceAndShadow-Screenshot.png)

## HOW IT WORKS

The light sources are treated as points and emit particles. The light particles that are not blocked by the screen help to expose a film-like surface, making it brighter. Rays can be drawn to show the exposure boundaries for each light source. A histogram reports the number particles that make it to the film locations as local intensity.

## HOW TO USE IT

Set the screen position (screen-x), the number of lights, and the ray-motion; press `setup` and then press `go`. For an exercise in the modeling class, we look at different `ray-motion` (straight, curve-left, and wiggle). The exercise is to gather evidence to support different models.

The `make-shadow-lines` function shows where the light is blocked by the screen and cannot expose the film.

## THINGS TO NOTICE

As the light rays get the film on the right side, the discreet points become brighter. The histogram shows the brightness for each of these discreet points. Think of these as pixels on a screen. Sometimes these discreet points are on the shadow boundary. In this case, the intensity might not match one's expectation. This is like a numeric round-off error.

## THINGS TO TRY

Try running with different number of light sources and the screen at different locations. Can you predict how the film will be exposed?

Try different `ray-motions`… How does the film expose? Does this match your expectations?

## NETLOGO FEATURES

A list is used for the light y-positions. The list is modified for an even number of lights.

When the sources create the shadow boundaries, two shapeless turtles are created. The shape has no features. The two are then differentiated by their `who` number. We look for the max `who` for the upper boundary and then the min `who` for the lower. 


## CREDITS AND REFERENCES

This model was developed with the creative juices of Stan Yoshinobu, Matt Moelter, Chance Hoellwarth of the Center for Excellence in Science and Math at California Polytechnic University, San Luis Obispo, Ca

## LICENSE

LightSourceAndShadow Model. CopyRight 2014 Vic Castillo

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>

This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.
## REPOSITORY

https://github.com/VicCastillo/LightSourceAndShadow


