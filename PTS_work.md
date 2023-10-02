# Effect of sugar length and number of sugars in PTS dynamics

Initially, we took a 1000 amino acid long fragment of the PTS region. Here we represented each of the amino acids with a single bead centered at its C<sub>&alpha;</sub> atom. Now, we added sugars to it using our own code, and make the structure as compact as possible by applying pulling. After pulling we tried to add more sugars, and added more sugars to it. Then I removed some sugars from the structure and appropriately modified the itp file to get difffferent degrees of glycosylation.

Initially each of the sugar chains were represented as four-bead chains, and the end bead has a negative charge.

## Effect of degree of glycosylation

### __Starting structures__

the initial structure with which the simulation was started are as follows:

<div style="display: flex;">
    <div style="flex: 33.33%; padding: 10px;">
        <h2>0% glycosylation</h2>
        <img src="GLY.DEGREE/sugar_0.00.png" alt="Image 1" style="width: 33.33%;">
    </div>
    <div style="flex: 33.33%; padding: 10px;">
        <h2>40% glycosylation</h2>
        <img src="GLY.DEGREE/sugar_0.40.png" alt="Image 2" style="width: 33.33%;">
    </div>
    <div style="flex: 33.33%; padding: 10px;">
        <h2>80% glycosylation</h2>
        <img src="GLY.DEGREE/sugar_0.80.png" alt="Image 3" style="width: 33.33%;">
    </div>
</div>


### __End structures__

As the simulations progressed in all of the cases we see the structures become more expanded as follows,

<div style="display: flex; justify-content: space-between;">
    <div>
        <h2>0% glycosylation</h2>
        <img src="GLY.DEGREE/sugar_0.00_last.png" alt="Image 1" style="width: 100%;">
    </div>
    <div>
        <h2>40% glycosylation</h2>
        <img src="GLY.DEGREE/sugar_0.40_last.png" alt="Image 2" style="width: 100%;">
    </div>
    <div>
        <h2>80% glycosylation</h2>
        <img src="GLY.DEGREE/sugar_0.80_last.png" alt="Image 2" style="width: 100%;">
    </div>
</div>

### __Radius of gyration and density of protein beads__

It seems the radius of gyration increases with the increasing degree of glycosylation. There are two things we need to consider. One is mass of the glycans make the PTS chain heavier, thus is fluctuates less as the number of sugars increases. At the same time, as the number of sugars increases, there are more electrostatics repulsions which make the chains to go away from each other.

![Image Alt Text](GLY.DEGREE/rg_plot_four_nead.png)

### __Distribution of the radius of gyration__


The distribution of the radius of gyration is as follows, it seems to be shifted towards the higher side and the general trend is the more degree of glycosylation the distribution is narrower. 

![Image Alt Text](GLY.DEGREE/rg_distribution_four_bead.png)



