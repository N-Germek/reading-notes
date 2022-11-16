# matplotlib

This is the leading 2D graphic tool for python users.

## IPython

The enhanced shell for python.features include: named inputs and outputs, access to shell commands, improved debugging, interactive matplotlib sessions with access to Matlab/Mathematica-like functionality.

## pyplot

Provides a convenient interface to matplotlib object oriented plotting library. Modeled after Matlab (TM).

## Getting Simple Plots

1. Get the sine and cosine of the function.

```python

X = np.linspace(-np.pi, np.pi, 256, endpoint=True)
C, S = np.cos(X), np.sin(X)
```

X is converted to a NymPy array with 256 values. C is the cosine and S is the sine.

2. to run the eample, you can run the code below.

```python

$ python exercice_1.py
```

You can customize properties and set defaults in matplotlib such as: figure size and dpi, line width, color and style, axes, axis and grid properties, text, font properties.

An example of customizing the cosine in blue and the sine in red is coded below:

```python
plt.figure(figsize=(10,6), dpi=80)
plt.plot(X, C, color="blue", linewidth=2.5, linestyle="-")
plt.plot(X, S, color="red",  linewidth=2.5, linestyle="-")
```

An example of setting limits to be able to see more of the graph is coded below:

```python
plt.xlim(X.min()*1.1, X.max()*1.1)
plt.ylim(C.min()*1.1, C.max()*1.1)
```

An example of setting ticks is below:

```python
plt.xticks( [-np.pi, -np.pi/2, 0, np.pi/2, np.pi])
plt.yticks([-1, 0, +1])
```

An example of setting tick labels is below:

```python
plt.xticks([-np.pi, -np.pi/2, 0, np.pi/2, np.pi],
       [r'$-\pi$', r'$-\pi/2$', r'$0$', r'$+\pi/2$', r'$+\pi$'])

plt.yticks([-1, 0, +1],
       [r'$-1$', r'$0$', r'$+1$'])
```

If you wanted to move spines, here is an example of what that would look like:

```python
ax = plt.gca()
ax.spines['right'].set_color('none')
ax.spines['top'].set_color('none')
ax.xaxis.set_ticks_position('bottom')
ax.spines['bottom'].set_position(('data',0))
ax.yaxis.set_ticks_position('left')
ax.spines['left'].set_position(('data',0))
```

An example of adding a legend would look like this:

```python
plt.plot(X, C, color="blue", linewidth=2.5, linestyle="-", label="cosine")
plt.plot(X, S, color="red",  linewidth=2.5, linestyle="-", label="sine")

plt.legend(loc='upper left', frameon=False)
```

If you wanted to annotate points, it would look something like this:

```python
t = 2*np.pi/3
plt.plot([t,t],[0,np.cos(t)], color ='blue', linewidth=1.5, linestyle="--")
plt.scatter([t,],[np.cos(t),], 50, color ='blue')

plt.annotate(r'$\sin(\frac{2\pi}{3})=\frac{\sqrt{3}}{2}$',
             xy=(t, np.sin(t)), xycoords='data',
             xytext=(+10, +30), textcoords='offset points', fontsize=16,
             arrowprops=dict(arrowstyle="->", connectionstyle="arc3,rad=.2"))

plt.plot([t,t],[0,np.sin(t)], color ='red', linewidth=1.5, linestyle="--")
plt.scatter([t,],[np.sin(t),], 50, color ='red')

plt.annotate(r'$\cos(\frac{2\pi}{3})=-\frac{1}{2}$',
             xy=(t, np.cos(t)), xycoords='data',
             xytext=(-90, -50), textcoords='offset points', fontsize=16,
             arrowprops=dict(arrowstyle="->", connectionstyle="arc3,rad=.2"))
```

Finally here is an example to fine tune the details so that your red and blue plot lines are not overpowering the tick marks on your code.

```python
for label in ax.get_xticklabels() + ax.get_yticklabels():
    label.set_fontsize(16)
    label.set_bbox(dict(facecolor='white', edgecolor='None', alpha=0.65 ))
```

## Things I want to know more about

## Resources

- > [Matplotlib Tutorial](https://github.com/rougier/matplotlib-tutorial)

## Links

- >[Advanced Software Development](README.md)
