+++
title = 'Ideas'
date = 2024-03-02T14:32:17-05:00
+++

A list of projects and plans for the future.

## Programming Projects

- [Project Euler](https://projecteuler.net)

### Digital Aquarium

This would be a... not a video game *per se*, but a simulation of some area of wilderness with populations of various animals. Each animal would have its own AI and would interact with its environment. There would be predator/prey relationships, animals would be born, age, and breed, and die, they would migrate, there would be a day/night cycle and a yearly cycle of seasons, and so on. The game would keep track of events and give the user summaries, and one could pull up population demographics and other reports. I was thinking ASCII graphics, like Dwarf Fortress.

### Hex Map Editor

I don't like the current options available for making world maps on a hexagonal grid for Dungeons and Dragons. I'd prefer a simple graphical interface that allows you to click-and-drag to fill areas with a preselected terrain option, saves files in a human-readable and human-editable plaintext format, and exports maps to images. The plaintext format is more important to me, and I would work on a tool that just takes the plaintext files as input and writes an image as output before I worked on a GUI for editing.

For the file format, it would need the following information:

- The width and height of the map.
- Whether the hexes are aligned horizontally or vertically.
- Whether the second row (or column) is indented or outdented relative to the first.
- The actual content of the map.
- A list of lists of hexes representing roads, rivers, etc.
- A list of hexes with names and descriptions of important locations.

As an example, a file could look like this:

```
    10,10,horizontal,indent
    ---
    AAAAAAAAAA
    AAAAnnnnnn
    AAnnn
    nnn    ~~
    n    ~~~
        ~~~TT
      TTTTTTT
    TTTTTTTTTT
    TTTTT
    TT
    ---
    5,4:city:"Crystalport"
```

This would code for a 10 by 10 map with horizontally aligned hexes, where the second row is indented relative to the first. The 'A's represent mountains, 'n's represent hills, '~'s represent water, and 'T's represent trees. The final line is an instruction to draw a "city" symbol at hex (5,4) and label it "Crystalport".

### Terrain Generation

This would be a heavy-duty terrain generator for voxel worlds like Minecraft, but using erosion to model realistic mountains, valleys, and meandering rivers. Mostly I want to code this for my own amusement.

### Medieval Demographics

This would just be an updated version of the procedure from S. John Ross's article [*Medieval Demographics Made Easy*](https://gamingballistic.com/wp-content/uploads/2018/11/Medieval-Demographics-Made-Easy-1.pdf), adding features I deem useful as I investigate it.

### Browser History Visualizer

I'm not a fan of the limited visualizations available in the current options.

### Counterpoint Solver

Yet another species counterpoint solver, but using plaintext input and output. I would like to use something like the following for input:

```
| A1 | A2 | G2 | F2 | E2 | D2 | C2 | B1 | D2 | C#1 | D2 |
| D1 | F1 | E1 | D1 | G1 | F1 | A1 | G1 | F1 | E1  | D1 |
```

## Textbooks to Study

I will probably never get around to the math and physics books, since I don't have a use for them in my job anymore.

### Computer Science

- Nystrom, [*Crafting Interpreters*](https://www.craftinginterpreters.com)
- Abelson & Sussman, [*Structure and Interpretation of Computer Programs*](https://mitp-content-server.mit.edu/books/content/sectbyfn/books_pres_0/6515/sicp.zip/index.html)
- Sussman & Wisdom, [*Structure and Interpretation of Classical Mechanics*](https://mitp-content-server.mit.edu/books/content/sectbyfn/books_pres_0/9579/sicm_edition_2.zip/book.html)

### Mathematics

- Cheng, *The Joy of Abstraction*
- Aluffi, *Algebra: Chapter 0*
- Munkres, *Topology*
- Rudin, *Principles of Mathematical Analysis*

### Physics

- Feynman, *Lectures on Physics*
- Goldstein, *Classical Mechanics*
- Jackson, *Classical Electrodynamics*
- Cohen-Tannoudji, *Quantum Mechanics*
- Reif, *Fundamentals of Statistical and Thermal Physics*
- Taylor & Wheeler, *Spacetime Physics*
