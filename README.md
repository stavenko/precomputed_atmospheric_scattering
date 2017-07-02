## Synopsis
This if a fork of original implementation of precomputed atmospheric
scattering. This fork is exclusively created to be build in mac os x.
### Differences to original code:

#### Pros:
 * Use of GLFW instead of GLUT. Now it's usabale on macs as well as windows and
     linux systems
 * contains fixes of shaders, which didn't work with original implementation:
   * Check for negative numbers in `sqrt`. This check helped to fix incorrect
       rendering
   * do not use use unattached textures as IN values in shader functions
#### Cons
 * Turned off keyboard controls as I didn't fixed all the implemetation, but
     only precomputed scattering code
 * Turned off display of helping message. 
 * Shaders code now is a little mess.
 

I can accept PRs, but have no interest in further development of this project.
Original Readme and detailed description i may find in original project.

## Building

Building command for the project is:

$ cd <root>/precomputed_atmospheric_scattering/
$ make demo

You will need to install at least `glfw` and `glew`. Feel free to ask quaestions.


## License

This project is released under the BSD license.

