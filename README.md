# day4-research_projects
Discussions and examples brought up by workshop attendants.
Discussions of `RSPt`'s features mentioned [here](http://www.physics.uu.se/research/materials-theory/ongoing-research/code-development/rspt-main/) might also be of interest.

### How to get RSPt's input file `symt.inp` 

#### 1. `.cif`-file + `cif2cell`
When starting a research project of a new material one can often find the crystal structure at [springer materials](https://materials.springer.com/search?searchTerm=CoFe2O4&oldPageNumber=1&totalNumberOfPages=2&autoRedirectTextSearch=false&substanceId=) (or some other database) and download it in a `.cif`-format. 

To convert the information in a `.cif`-format to RSPt's `symt.inp`-format, one can use a open-source software called [`cif2cell`](https://sourceforge.net/projects/cif2cell/).
Just type:
```bash
cif2cell -p rspt --rspt-new XXX.cif 
```
to generate the corresponding `symt.inp`-file containing the crystal-structure information.
Continue with the simulation setup and then run and enjoy RSPt!

#### 2. Manually write it
Also works fine of course.

