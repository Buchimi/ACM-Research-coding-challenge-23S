# ACM Research coding challenge (Spring 2023)

## Libraries used
numpy
pandas
scikit-learn
matplotlib

## Problems explored
### A potential relationship between the radius of a star and it's mass.
By using the mass-luminosity relationship, I was able to approximate the masses of each main sequence star.
I didn't use this formula for stars outside the main sequence.
This is because I wasn't confident in the presence of such a relationship, as the sun is a main sequence star and this relation depends on the star's mass being relatable to the sun

![mass vs radius](https://github.com/Buchimi/ACM-Research-coding-challenge-23S/blob/main/mass_vs_radius_of_stars.png)

I interprete this as a positive correletion but I don't have an explanation for the stars at the top right. Possibly a flaw in using the formula to approximate the mass for the wrong type of star

### The energy density of stars
As our civilization continues to advance, the question of how we get sustainable energy looms in the distance. Given the data, I decided to look for a relationship between a star's color and its energy density (how much energy is emitted per surface area)

We should be able to (in theory) generate the most power per surface area of solar cells, if we focus on stars with a high energy-to-surface area ratio. Which eventually boils down to a luminosity per radius ratio.

Surface area is found with 2 * pi * radius
energy is substituted directly with luminosity

I compared these two variables with a box plot and found out that blue stars are the most energy dense.
![star color vs energy density](https://github.com/Buchimi/ACM-Research-coding-challenge-23S/blob/main/star_color_vs_energy_density.png)

## Limitations
- incorrect use of the mass-luminosity relation
- The stars in the mass vs radius graph at the upper left are unaccounted for. 

## Challenge
- Learning all these libraries. I have never used them before (except matplotlib) and playing around with them was a new experience for me
- matplotlib 3d is hard to understand. I couldn't figure out how to represent gravitational curvature in 3d space using numpy arrays

## What I wanted to explore
- A representation of stars and how their gravitational curvature of space-time relates to their mass
- Predicting the lifetime of stars based on their current features
