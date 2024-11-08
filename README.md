# Virtual Garden Management Program

This program allows users to manage a virtual garden by performing actions like planting, growing, harvesting, picking, and cutting various types of plants. Users can interact with the garden through various commands to simulate its state over time.

## How to Use

To run the program, specify the input file name as a command-line argument:

```bash
java App myGarden.in

# Virtual Garden Management Program

## Input File Format

Commands should be written on separate lines. Coordinates (x, y) are zero-indexed. The garden grid supports a maximum width of 80 characters, with up to 16 plots horizontally.

## Commands Overview

# PLANT (x,y) <type>
# Plants a specific type at (x, y).
# Example: PLANT (0,0) rose
PLANT = "PLANT (x,y) <type>"

# PRINT
# Displays the current state of the garden.
# Example: PRINT
PRINT = "PRINT"

# GROW <num>
# Increases growth of all plants by the specified number.
# Example: GROW 1
GROW_NUM = "GROW <num>"

# GROW <num> (x,y)
# Grows the plant at (x, y) by a given amount.
# Example: GROW 1 (2,3)
GROW_COORD = "GROW <num> (x,y)"

# GROW <num> <type>
# Increases growth of all plants of a specified type.
# Example: GROW 1 rose
GROW_TYPE = "GROW <num> <type>"

# HARVEST
# Removes all vegetables from the garden.
HARVEST = "HARVEST"

# HARVEST (x,y)
# Harvests the vegetable at (x, y) if applicable.
# Example: HARVEST (2,3)
HARVEST_COORD = "HARVEST (x,y)"

# HARVEST <type>
# Harvests all vegetables of a specified type.
# Example: HARVEST tomato
HARVEST_TYPE = "HARVEST <type>"

# PICK
# Removes all flowers from the garden.
PICK = "PICK"

# PICK (x,y)
# Picks the flower at (x, y) if applicable.
# Example: PICK (2,3)
PICK_COORD = "PICK (x,y)"

# PICK <type>
# Picks all flowers of a specified type.
# Example: PICK rose
PICK_TYPE = "PICK <type>"

# CUT
# Removes all trees from the garden.
CUT = "CUT"

# CUT (x,y)
# Cuts the tree at (x, y) if applicable.
# Example: CUT (2,3)
CUT_COORD = "CUT (x,y)"

# CUT <type>
# Cuts all trees of a specified type.
# Example: CUT PINE
CUT_TYPE = "CUT <type>"


##Example Input File

rows: 1
cols: 1
PLANT (0,0) apple
PRINT
GROW 1
PRINT
