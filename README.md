### gen_noise ###

a port of some noise functions to be used in jit.gl.pix or jit.gen in 
max/msp

note : noises other than voronoi based by default return signed values -1 
to 1. you can set to unsigned by using function parameter sgn

e.g. simplex_noise(p3, sgn=0);

these make use of function parameters

see code/gen_noise.genexpr 

for instance:
multifractal(point, H=1.5, lacunarity=1.5, frequency=1, octaves=6, offset=.85) 

right now these are comparable to the following (see 
examples/gen_noise_bfg_comparison.maxpat for usage)



perlin_noise -> noise.perlin 

simplex_noise -> noise.simplex

cell_noise -> noise.cell

checker_noise -> noise.checker

ridged_multifractal -> fractal.multi.rigid

hybrid_multifractal-> fractal.multi.hybrid

fbm -> fractal.fbm

multifractal -> fractal.multi

hetero_terrain-> fractal.hetero

voronoi_noise -> noise.voronoi

voronoi_crackle -> noise.voronoi.crackle

voronoi_smooth -> noise.voronoi.smooth

voronoise -> noise.voronoise,

voronoi_id -> noise.voronoi.id,

distorted use distorted function with noise inputs

distorted.2axis use distorted2axis function with noise inputs

curl_noise

worley_noise



