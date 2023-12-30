
![ascii-text-art](https://github.com/zelhajou/fractol/assets/39954629/8c399f6f-09da-45f2-96ff-05e990046bc9)

## Description
Fract-ol is a computer graphics exploration project centered around the beauty and complexity of fractals. Using the C programming language and the [MiniLibX](https://harm-smits.github.io/42docs/libs/minilibx) library, this project aims to render stunning visual representations of the Julia and Mandelbrot fractal sets. It serves as a practical application of complex numbers, computer graphics optimization, and event handling in graphics programming.

## Installation
To install Fract'ol, clone the repository and compile the source code using the provided Makefile.

```bash
git clone [repository-link]
cd fractol
make
```
Ensure that the MiniLibX library is installed on your system before compiling.

## Usage
Run the program with the following command:

```c
./fractol [fractal-type]
```
Replace **[fractal-type]** with either **Julia** or **Mandelbrot** to view the respective fractal set.

## Explination :
\sum  \because 
In mathematics, there are many different types of geometry, each exploring shapes and dimensions in unique ways. Among these, fractal geometry is one of the most intriguing.

**Fractal Geometry** deals with shapes that look similar at any scale. This means that if you look at a small part of the shape, you will find it resembles the entire shape. Imagine a tree, where the smaller branches branch out in a way that mimics the whole tree. Fractals are not just beautiful drawings; they are crucial in science and mathematics to understand complex patterns in nature.


<img width="540" alt="Screen Shot 2023-12-29 at 4 09 18 PM" src="https://github.com/zelhajou/fractol/assets/39954629/640227c8-133c-4f5d-963d-4daa2cc88858">


Among the most famous fractal sets are the Julia and Mandelbrot sets:

- **Julia Set:** Known for its complexity and beauty, it consists of points that generate complex fractal shapes when certain mathematical operations are applied to them.
- **Mandelbrot Set:** Recognized for its distinctive shape, it is a complex example of fractals, representing a set of points in the mathematical space that exhibit repeating patterns when magnified.

### Calculating the Julia and Mandelbrot Sets

### Complex Numbers
**Complex Numbers** are numbers that combine real and imaginary parts. A complex number is written as `a + bi`, where:
- `a` is the real part.
- `bi` is imaginary part.
- `i` is the imaginary unit, defined as the square root of -1, so `i^2 = -1`.

https://www.mathsisfun.com/numbers/complex-numbers.html

#### Mandelbrot Set:
1. Choose a complex number `c`.
2. Start with `z_0 = 0`.
3. Repeatedly apply the formula: `z_{n+1} = z_n^2 + c`.
4. If the magnitude of `z_n` (|`z_n`|) remains less than or equal to 2 after many iterations, then `c` is part of the Mandelbrot set.
5. If |`z_n`| exceeds 2 at any step, `c` is not part of the Mandelbrot set.

#### Julia Set Calculation:
1. Choose a fixed complex number `c`.
2. Choose `z_0` as your starting point.
3. Repeatedly apply the formula: `z_{n+1} = z_n^2 + c`.
4. If the magnitude of `z_n` (|`z_n`|) stays less than or equal to 2 after many iterations, then `z_0` is part of the Julia set.
5. If |`z_n`| exceeds 2, `z_0` is not part of the Julia set.

Note: In these formulas, `z_n` and c are complex numbers, and `z_{n+1}` represents the complex number obtained after applying the formula to `z_n`.

<img width="520" alt="Screen Shot 2023-12-29 at 4 09 18 PM" src="https://github.com/zelhajou/fractol/assets/39954629/2fbedc75-f234-4b93-8686-6a10ac71b9aa">




### Other Types of Geometry in Mathematics
1. **Euclidean Geometry:** Deals with shapes in flat (2D) or three-dimensional (3D) space.
2. **Non-Euclidean Geometry:** Includes spherical geometry and hyperbolic geometry.
3. **Analytic Geometry:** Uses coordinates and equations to describe shapes.
4. **Algebraic Geometry:** Studies shapes using algebra.
5. **Topological Geometry:** Deals with shapes in higher dimensions and complex spaces.
6. **Differential Geometry:** Uses calculus to study geometric properties.


# Mandelbrot sets
<img width="320" alt="Screen Shot 2023-12-29 at 4 09 18 PM" src="https://github.com/zelhajou/fractol/assets/39954629/fa2a496f-c941-4d1c-97d7-e54136d2b654">

# Julia sets

| | | |
|:-------------------------:|:-------------------------:|:-------------------------:|
| Julia set for fc, c = −0.7269 + 0.1889i <br> ![Julia Set -0.7269 + 0.1889i](https://github.com/zelhajou/fractol/assets/39954629/9967eae3-844c-408c-9048-77c656882f15) | Julia set for fc, c = (φ − 2) + (φ − 1)i = −0.4 + 0.6i <br> ![Julia Set -0.4 + 0.6i](https://github.com/zelhajou/fractol/assets/39954629/bacc447b-0b33-44a8-aaf0-0a158a25ac29) | Julia set for fc, c = 0.35 + 0.35i <br> ![Julia Set 0.35 + 0.35i](https://github.com/zelhajou/fractol/assets/39954629/5ba7b8c7-8a51-40bb-9d88-17d8cb826889) |
| Julia set for fc, c = 0.285 + 0.01i <br> ![Julia Set 0.285 + 0.01i](https://github.com/zelhajou/fractol/assets/39954629/8edb61b7-d8f1-4535-86f1-bfbb69be863d) | Julia set for fc, c = −0.8 + 0.156i <br> ![Julia Set -0.8 + 0.156i](https://github.com/zelhajou/fractol/assets/39954629/0da1efbb-f0a8-40b4-b381-cc7fdf2ecc25) | Julia set for fc, c = 0.4 + 0.4i <br> ![Julia Set 0.4 + 0.4i](https://github.com/zelhajou/fractol/assets/39954629/5662bcc7-c743-47af-8684-e5b15b571a20) |
| Julia set for fc, c = −0.835 − 0.2321i <br> ![Julia Set -0.835 - 0.2321i](https://github.com/zelhajou/fractol/assets/39954629/843ff757-c0fa-40eb-b386-9f15ca9461d3) | Julia set for fc, c = 0.285 + 0i <br> ![Julia Set 0.285 + 0i](https://github.com/zelhajou/fractol/assets/39954629/ddd6896e-dfae-4f22-bee3-71eba91003c7) | |

<!--
Julia set for fc, vc = −0.7269 + 0.1889i

<img width="787" alt="Screen Shot 2023-12-29 at 11 44 18 PM" src="https://github.com/zelhajou/fractol/assets/39954629/9967eae3-844c-408c-9048-77c656882f15">

Julia set for fc, c = (φ − 2) + (φ − 1)i = −0.4 + 0.6i

<img width="795" alt="Screen Shot 2023-12-29 at 5 06 49 PM" src="https://github.com/zelhajou/fractol/assets/39954629/bacc447b-0b33-44a8-aaf0-0a158a25ac29">

Julia set for fc, c = 0.35 + 0.35i

<img width="793" alt="Screen Shot 2023-12-29 at 4 19 33 PM" src="https://github.com/zelhajou/fractol/assets/39954629/5ba7b8c7-8a51-40bb-9d88-17d8cb826889">

Julia set for fc, c = 0.285 + 0.01i

<img width="793" alt="Screen Shot 2023-12-29 at 4 21 21 PM" src="https://github.com/zelhajou/fractol/assets/39954629/8edb61b7-d8f1-4535-86f1-bfbb69be863d">

Julia set for fc, c = −0.8 + 0.156i

<img width="795" alt="Screen Shot 2023-12-29 at 4 16 06 PM" src="https://github.com/zelhajou/fractol/assets/39954629/0da1efbb-f0a8-40b4-b381-cc7fdf2ecc25">

Julia set for fc, c = 0.4 + 0.4i

<img width="787" alt="Screen Shot 2023-12-29 at 4 10 05 PM" src="https://github.com/zelhajou/fractol/assets/39954629/5662bcc7-c743-47af-8684-e5b15b571a20">

Julia set for fc, c = −0.835 − 0.2321i

<img width="794" alt="Screen Shot 2023-12-29 at 4 15 21 PM" src="https://github.com/zelhajou/fractol/assets/39954629/843ff757-c0fa-40eb-b386-9f15ca9461d3">

Julia set for fc, c = 0.285 + 0i

<img width="796" alt="Screen Shot 2023-12-29 at 5 09 31 PM" src="https://github.com/zelhajou/fractol/assets/39954629/ddd6896e-dfae-4f22-bee3-71eba91003c7">

-->

