# ferncal: A database of fossils for molecular dating of the fern tree of life

[![DOI](https://zenodo.org/badge/465086693.svg)](https://zenodo.org/badge/latestdoi/465086693)

ferncal is a database of fossil specimens for fossil-calibrated molecular dating of ferns.

This dataset was originally compiled for the following paper:  
- Nitta JH, Schuettpelz E, Ramírez-Barahona S, Iwasaki W. An open and continuously updated fern tree of life (FTOL)

## Phylosophy

The main aim of constructing this fossil calibration list is to have an open resource that can be continually updated based on community feedback. We encourage users to propose additions to the list or changes to the taxonomic assignment of particular fossils.

The general philosophy behind this list is to include fossils whose metadata are available (e.g., the original publication, locality, specimen numbers), thus providing the opportunity to re-assess the fossil and its taxonomic affinitites based on updated taxonomic knowledge. Thus, fossil-calibration of molecular trees using our list of fossils has several advantages:
- Calibration points based on individual specimens, which are useful for FBD-type dating.
- Continuous update of the list (e.g., corrections or additions).
- Re-assessment of taxonomic affinities based on current knowledge.

## Data format

The fossil data are contained in [fern_fossils.csv](fern_fossils.csv).
For a description of each variable (column), see [fern_fossils_metadata.csv](fern_fossils_metadata.csv).

Some of the variables use (pandoc-style) [markdown formatting](https://pandoc.org/MANUAL.html#pandocs-markdown); e.g., species names surrounded by asterisks to indicate they should be in italics and reference keys preceded by the `@` symbol.
This is to facilitate printing the data as a formatted PDF document. 
Columns including markdown formatting are `node_calibrated`, `full_taxon_name`, `affinities`, `notes_on_affinities`, and `notes_on_age`.

The reference data (publication for each fossil) are contained in [fern_fossils.bib](fern_fossils.bib) (bibtex format).

## Citing

If you use this database, please cite it!

Here is an example:

    FTOL working group. (2022). ferncal: A database of fossils for molecular dating of the fern tree of life v1.0.0. https://doi.org/10.5281/zenodo.6395322

The example DOI above is for the overall database.

Here is the latest DOI, which you should cite if you are using the latest version of the database:

[![DOI](https://zenodo.org/badge/465086693.svg)](https://zenodo.org/badge/latestdoi/465086693)

You can find DOIs for older versions by viewing the "Releases" menu on the right.
## Notes to users

- Each fossil has a unique identifier (`n_fos`). In order to keep track of fossils calibrations (both here and in publications), we strongly encourage users to mention fossils using this identifier.  
- The addition of new fossils is contingent on users providing the full reference (in bibtex format) to the original publication where the material is described.  
- To keep track of the history of use of these fossils, if a taxonomic change is needed (e.g., change in generic circumscription) a note on the proposed change will be added while keeping track of the original taxonomic assignment.  
- Deletions to fossil list will not be considered, but in particular cases a note of caution will be appended.
- We recommend a plain-text editor for editing (e.g., VS-code, BBEdit), not Excel, since Excel may result in unexpected changes to the CSV format.
- The list is in (continuous) development. Thus, at any given time fossil entries might be incomplete.

## License

- [CC0](LICENSE)