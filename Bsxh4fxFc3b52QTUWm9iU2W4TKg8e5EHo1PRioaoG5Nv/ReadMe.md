Bsxh4fxFc3b52QTUWm9iU2W4TKg8e5EHo1PRioaoG5Nv
Sinco Drum Pad 16
Reading the cheap Sinco Drum Pad 16.


Find here an example of how you can read the Drum Pad 16.

The one I bought:
https://www.amazon.com.be/-/en/dp/B0DY1KYS2W

A 4×4 pad-grid tool for GOMI would be nice for DIY projects like this, since 16 buttons can fit on an ESP32.

The M-VAVE format used by the Sinco has a default behavior: there is a velocity value of 64 when a button is released.

That is the reason for this demo.

I should add code that allows an input/output event to be triggered based on a given text image.

The exact pattern is:

```text
1100
1100
0000
0000
```

Whatever the rest contains, for example:

```text
11--
----
----
```

The first line must be:

```text
1100
----
----
----
```

Is exacly
```
1100
1100
0000
0000
```

What ever the rest
```
11--
----
----
```

First line must be
```
1100
----
----
----
```
