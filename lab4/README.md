What is a formula to get the x coordinate of the texture given a u value of the uv coordinate (a value between 0 and 1)?
Let a = the x dimension of sample size (8 in this case)
x = u * a

What is a formula to get the y coordinate of the texture given a v value of the uv coordinate (a value between 0 and 1)?
take the v value
Let b = the y dimension of sample size (8 in this case)
y = b - (v * b)

What color is sampled from the texture at the uv coordinate (0.375, 0.25)? (sample from the image based on the number your formula gives you i.e. (1, 0) (x, y) is blue)

(3, 5) is blue

Lab4 demo video link: https://drive.google.com/file/d/1CxgWtLFWyjuDH7QX1lP6Yoa8CZa5qVcu/view?usp=sharing

Part 1 (Center cube) Texture A (uses three.js built in texture functionality)
Part 1 (Left cube) Texture A & Normal Map A (uses three.js built in texture functionality)
Part 1 (Bottom cube) Texture B & Normal Map B (new texture/normal map combo using built in three.js functionality)
Part 2 (Right cube) Texture C (load this texture with shaders, as we worked through in the lab together)
Part 2 (Top cube) Texture D (tile this texture at least by showing a 2x2 grid) - Was not able to figure out how to make a 2x2 grid, but was able to stretch out the brick texture by using mod with the x and y coordinates of vUv - vec2(mod(vUv.x, .5), vUv.y);


