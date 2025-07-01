import math
# This is very basic and doesn't take several variables into account such as how "evaporated" the black hole is, Temperature, Entropy, Schwarzschild radius, Surface area, Nominal luminosity, Peak photons, ect. 
# I should really just make a new calculator.
# Credits: https://github.com/jellyfish445, https://en.wikipedia.org/wiki/Hawking_radiation, https://en.wikipedia.org/wiki/Black_hole

# Constants (SI units)
hbar = 1.0545718e-34     # Reduced Planck constant (J·s)
c = 2.99792458e8         # Speed of light (m/s)
G = 6.67430e-11          # Gravitational constant (m^3/kg/s^2)
pi = math.pi             # Pi is pi

# Black hole parameters
mass = 1e11              # Black hole mass in kg (smaller is more energy) -if you're going to do lbs, don't. KG is used in math!
time = 30                # Time interval in seconds -Portion of time you're looking at

# Hawking radiation power formula thing
def hawking_radiation_power(mass_kg):
    numerator = hbar * c**6
    denominator = 15360 * pi * G**2 * mass_kg**2
    return numerator / denominator  # Power in watts (J/s)

# Calculate powah and energy
unlimitedpowa = hawking_radiation_power(mass)
energy = power * time

# Output results
print(f"Hawking Radiation Power for {mass:.1e} kg black hole: {unlimitedpowa:.3e} W")
print(f"Energy emitted in {time} seconds: {energy:.3e} J")
