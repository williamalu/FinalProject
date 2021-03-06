# CompArch Final Project: Verilog Intersection Controller
William Lu and Kathryn Hite

## Materials

The report for this project can be found in VerilogIntersectionController.pdf


## Run Instructions

There are currently a few bugs left in the intersection_controller testbench that create timing problems.  The current visualization simulation is based off of testbench output without these additions, and the instructions below still run in the current state.

To build and visualize an intersection:

**Using the script:**

Run the following to see the intersection visualization

```
./full_intersection.sh
```

**Using the individual components:** 

you can first run the intersection_test.t.v file using the following terminal command:

```
iverilog -o intersection_test intersection.t.v
```

This builds a test case of the intersection and outputs the data to a text file with all of the light states throughout the test.  Running the visualization.py file reads those results and displays them as a model of an intersection.  