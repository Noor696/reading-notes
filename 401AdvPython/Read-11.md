## Read 11 - Data Visualization

## matplotlib-tutorial

[matplotlib-tutorial](https://github.com/rougier/matplotlib-tutorial#introduction)

* **matplotlib** is probably the single most used Python package for 2D-graphics. It provides both a very quick way to visualize data from Python and publication-quality figures in many formats.

* **IPython:**
    
    - enhanced interactive Python shell that has lots of interesting features (input - output)

    - access to shell commands

    - improved debugging and much more.

    - **allows interactive matplotlib sessions that have Matlab/Mathematica-like functionality.**

* **pyplot:**

    - provides a convenient interface to the matplotlib object-oriented plotting library.
    
    - modeled closely after Matlab(TM).

    - Matplotlib comes with a set of default settings that allow customizing all kinds of properties. 

    - You can control the defaults of almost every property in matplotlib: (figure size and dpi, line width, color and style, axes, axis and grid properties, text and font properties and so on.)

* Changing colors and line widths on matplotlib: (ex:)
    
    - plt.figure(figsize=(10,6), dpi=80)
    - plt.plot(X, C, color="blue", linewidth=2.5, linestyle="-")

* Setting limits : (ex:)

    - plt.xlim(X.min()*1.1, X.max()*1.1)

* Setting ticks in axis: (ex:)
    - plt.xticks( [-np.pi, -np.pi/2, 0, np.pi/2, np.pi])
    - plt.yticks([-1, 0, +1])

* also we can do defferante thing(Setting tick labels, Moving spines, Adding a legend, Annotate some points, Devil is in the details)

*  We can have more control over the display using figure, subplot, and axes explicitly.
    - A figure in matplotlib means the whole window in the user interface. Within this figure there can be subplots.

    - subplot positions the plots in a regular grid

    - axes allows free placement within the figure. Both can be useful depending on your intention
    
    