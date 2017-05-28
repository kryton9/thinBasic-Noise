## thinBasic-Noise

Based on information from http://paulbourke.net/texture_colour/perlin/

SeedNoise(seed): seed is an unsigned integer value used to seed the random generator used by the noise function.

Noise(scale, x, y, alpha, beta, n): function to manually fill an array of points and an array of colors with noise.

  scale > 0 and < 1   0.01 is a good start
  
  alpha start With 2, then <2 rougher, >2 smoother 
  
  beta start with 2, <2 zooms in and harsher, >2 zooms out and adds to the noise
  
  n is either 1, 2, 3 or 4 it is the number of layers of detail, lower is bigger detail
  
  n > 4 should make no noticeable difference
  
FillNoiseArray(scale, width, height, points, colors, alpha, beta, n) this is the function you want to use most of the time.

thinBasic forums: http://www.thinbasic.com/community/forum.php
