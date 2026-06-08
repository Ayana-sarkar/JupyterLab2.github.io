# JupyterLab2.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mastering JupyterLab</title>
    <style>
        /* Modern Reset & Variables */
        * {
            margin: 0;
            padding: 0;
            box-box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        :root {
            --bg-color: #0f172a;
            --card-bg: #1e293b;
            --accent-orange: #f97316;
            --accent-blue: #38bdf8;
            --text-main: #f8fafc;
            --text-muted: #94a3b8;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
        }

        /* Navbar */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.5rem 10%;
            background-color: rgba(15, 23, 42, 0.8);
            backdrop-filter: blur(10px);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--text-main);
        }
        .logo span {
            color: var(--accent-orange);
        }
        .nav-links a {
            color: var(--text-muted);
            text-decoration: none;
            margin-left: 2rem;
            transition: color 0.3s;
        }
        .nav-links a:hover {
            color: var(--accent-blue);
        }

        /* Hero Section */
        .hero {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 5rem 10%;
            min-height: 80vh;
        }
       .hero-content, [class*="hero"] {
          width: 100% !important;
           max-width: 950px !important; 
           margin: 0 auto !important;  
           padding: 40px 20px !important;
          text-align: left !important;  
        }

    .hero-content h1 {
         font-size: 3.5rem;
         line-height: 1.2;
         margin-bottom: 1.5rem;
        }

     .hero-content h1 span {
         color: var(--accent-orange);
       }


     .hero-content p {
          font-size: 1.2rem;
         color: var(--text-muted);
         margin-bottom: 2rem;
         max-width: 800px; 
       }
       .btn {
            display: inline-block;
            background: linear-gradient(135deg, var(--accent-orange), #ea580c);
            color: white;
            padding: 0.8rem 2rem;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 20px rgba(249, 115, 22, 0.4);
       
        /* Interactive Code Box Demo */
        .hero-visual {
            max-width: 45%;
            width: 100%;
        }
        .code-box {
            background-color: var(--card-bg);
            border-radius: 8px;
            padding: 1.5rem;
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
            border: 1px solid #334155;
        }
        .code-header {
            display: flex;
            gap: 0.5rem;
            margin-bottom: 1rem;
        }
        
        .code-input {
            color: var(--accent-blue);
            font-family: 'Courier New', Courier, monospace;
            margin-bottom: 1rem;
        }
        .code-output {
            background-color: #0f172a;
            padding: 1rem;
            border-radius: 4px;
            border-left: 4px solid var(--accent-orange);
            font-family: monospace;
        }

        /* Curriculum Section */
        .curriculum {
            padding: 5rem 10%;
            background-color: #0b111e;
        }
        .curriculum h2 {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
        }
        .grid,.row, [class*="card-container"], [class*="wrapper"]{
            display:flex !important;
            flex-direction: column !important;
            align-items: center !important;
            width: 100% !important; 
        }
        .card,[class*="box"], [class*="item"]{
            background-color: var(--card-bg);
            width: 100% !important;
            max-width: 800px !important;
            margin-bottom: 24px !important; 
            padding: 24px !important;
        }
        .card:hover {
            transform: translateY(-5px);
        }
        .card h3 {
            color: var(--accent-blue);
            margin-bottom: 1rem;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2rem;
            color: var(--text-muted);
            border-top: 1px solid #1e293b;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .hero {
                flex-direction: column;
                text-align: center;
                padding-top: 2rem;
            }
            .hero-content {
                max-width: 100%;
                margin-bottom: 3rem;
            }
            .hero-visual {
                max-width: 100%;
            }
            .nav-links {
                display: none; /* Keep it simple for mobile */
            }
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">🚀 Learn<span>Jupyter</span></div>
        <div class="nav-links">
            <a href="Environmental Management.pdf">ENVS</a>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
        </div>
    </nav>

    <section class="hero">
            <a href="https://ayana-sarkar.github.io/Home2.github.io/" class="btn">Basic</a>
            <a href="https://ayana-sarkar.github.io/JupyterLab4.github.io/" class="btn">Plotting with List</a>
            <a href="https://ayana-sarkar.github.io/JupyterLab5.github.io/" class="btn">Plotting with Arrays</a>
            <a href="https://ayana-sarkar.github.io/JupyterLab2.github.io/" class="btn">Interpolation</a>
            <a href="https://ayana-sarkar.github.io/JupyterLab1.github.io/" class="btn">Special func</a>
         <div class="hero-content">
            <h1> Interpolation</h1>
            <p>In data science, scientific computing, and engineering, interpolation is a mathematical method used to estimate unknown values that fall between known data points. </p>
         </div>
    </section>

    <section id="curriculum" class="curriculum">
        <div class="grid">
            <div class="card">
                <h2>1.Polynomial Interpolation</h2>
                <img src="Screenshot 2026-04-19 232319.png" alt="Data Visualization" class="box-image">
                <p>In NumPy, np.poly1d is a class used to conveniently handle and manipulate one-dimensional polynomials. Instead of forcing you to manually write out mathematical formulas like y =a n x n + an-1 xn-1+.....+ a0, np.poly1d takes an array of coefficients and transforms them into a callable function.<br> 
                Because we have 7 data points and chose a polynomial degree of len(x) - 1 (which is 6), the resulting curve will perfectly pass through every single one of your data points.<br> 
                Line 3: np.polyfit calculates the optimal coefficients for a 6th-degree polynomial that fits your 7 data points (x, y).It returns an array of 7 numbers representing the coefficients (from the highest power x6 down to the constant term).<br>
                Line4: This line wraps those raw coefficients into a poly1d object. Now, ploy acts exactly like a mathematical function, f(x). <br> 
                Line 5-6: np.linspace creates 100 evenly spaced points between your minimum x(1) and maximum x (7). By writing ploy(x_new), you are passing all 100 of those new x coordinates into your polynomial function. It instantly calculates the 100 corresponding y values (y_new). 
                Line 7-8: Finally, Matplotlib plots your original points as red circles ('ro') and the smoothly calculated x_new and y_new values as a blue line ('b-').
                <img src="Screenshot 2026-04-19 232341.png" alt="Data Visualization" class="box-image"></p>
            </div>
            <div class="card">
                <h2>2.</h2>
                <img src="Screenshot 2026-04-19 232549.png" alt="Data Visualization" class="box-image">
                <p>Line 1: np.polyfit(x, y, 3) changes the degree to 3. This calculates the mathematical coefficients of a 3rd-degree polynomial (y = ax^3 + bx^2 + cx + d) that minimizes the squared distance between the curve and your 7 red data points. It saves an array of 4 numbers [a, b, c, d] into the variable coeffs.<br> 
                Line 2: It takes that array of 4 coefficients and converts it into a convenient, executable Python function named ploy (representing equation f(x)).<br> 
                Now we can pass any x value into ploy to quickly get the predicted y value on the blue curve.<br>
                </p>
            </div>
            <div class="card">
                <h2>3.1D Interpolation</h2>
                <img src="Screenshot 2026-04-19 232613.png" alt="Data Visualization" class="box-image">
                <img src="Screenshot 2026-04-19 232753.png" alt="Data Visualization" class="box-image">
                <p>By setting kind='linear', we are telling SciPy to perform piecewise linear interpolation.<br> 
                f = interpolate.interp1d(x, y, kind='linear')<br> 
                we feed interp1d raw data arrays (x and y).<br> 
                yn = f(xn): here f looks at each number in xn, figures out which two original data points it falls between, calculates the straight-line height at that exact spot, and saves the results into yn.<br>
                <img src="Screenshot 2026-04-19 232802.png" alt="Data Visualization" class="box-image"></p>
            </div>
            <div class="card">
                <h2>4.</h2>
                <img src="Screenshot 2026-04-19 233226.png" alt="Data Visualization" class="box-image">
                <p>Setting kind='nearest' switches the behavior to Nearest-Neighbor Interpolation. Instead of drawing smooth curves or connecting the dots with straight diagonal lines, the function f acts like a strict decision-maker that assigns values based purely on proximity.<br> 
                When a new coordinate (xn) is passed into the function f, it looks for Which original x data point is closest to this new input. It finds the nearest known point.It adopts that exact known point's $y$ value completely. <br> 
                Because it does not average the points or transition smoothly between them, the resulting graph will look like a series of sharp steps or a jagged staircase.<br> 
                <img src="Screenshot 2026-04-19 233239.png" alt="Data Visualization" class="box-image"></p>
            </div>
            <div class="card">
                <h2>5.Spline Interpolation</h2>
                <p>A spline is composed of polynomial functions connected by knots and provides a stable and extended method of interpolation. The analytical form is useless for modeling, but the data returned are fast and reliable. <br></p>
          <img src="Screenshot 2026-04-19 233401.png" alt="Data Visualization" class="box-image">
           <img src="Screenshot 2026-04-19 233412.png" alt="Data Visualization" class="box-image">
           <img src="Screenshot 2026-04-19 233602.png" alt="Data Visualization" class="box-image">
           <p>kind='quadratic' (Quadratic Spline): SciPy fits a 2nd-degree polynomial (ax^2 + bx + c) between every neighboring pair of points. It ensures that the segments match up perfectly at the data points and that the slope (first derivative) is continuous where they touch.<br> 
           kind='cubic' (Cubic Spline): SciPy fits a 3rd-degree polynomial (ax^3 + bx^2 + cx + d) between every pair of points. It ensures that both the slope and the curvature (second derivative) match up seamlessly where the segments meet. This creates an incredibly natural, fluid curve.<br></p>
           <img src="Screenshot 2026-04-19 233612.png" alt="Data Visualization" class="box-image">
           </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 LearnJupyter Course. Built for future Data Scientists.</p>
    </footer>

</body>
</html>
