Uppmax maintains local copies of the full set of NCBI Taxonomy databases
(<https://www.ncbi.nlm.nih.gov/guide/taxonomy/>).  Note that:

* The local copies are found at `/sw/data/uppnex/ncbi_taxonomy/latest`
* This also contains the subdirectories `accession2taxid` and `biocollections` containing those databases, see the tables below for their contents
* `latest` is a symbolic link to a directory named from the date of the most recent update
* There is also a subdirectory `download` containing the files as downloaded from NCBI
* The installation of new versions begins **Sunday of each week at 00.10**.  The update may take several minutes up to an hour, depending on network speeds.
* When new versions are successfully installed, the `latest/` symbolic link is updated to point to the new dated directory
* The previous version of the taxonomy databases are removed when the new versions have completed installation

See the links for each database for specifics on file format and contents.
Many tools know how to make use of these databases; follow each tool's specific
instructions.  The files can be found in the indicated directories.

The databases available within `/sw/data/uppnex/ncbi_taxonomy/latest` are
below.  For more on each, see the links.

**Name** | **Source** | **Notes**
-----|------|--------
**taxdump** | [NCBI][taxdump] | NCBI taxonomic database, in multiple **.dmp** files (see link)
**taxcat** | [NCBI][taxcat] | NCBI taxonomic categories, in **categories.dmp** (see link)
**gi_taxid_nucl.dmp** | [NCBI][gi_taxid] | Mappings of nucleotide GI to taxid (DEPRECATED)
**gi_taxid_nucl_diff.dmp** | [NCBI][gi_taxid] | Differences between this and previous gi_taxid_nucl.dmp (DEPRECATED)
**gi_taxid_prot.dmp** | [NCBI][gi_taxid] | Mappings of protein GI to taxid (DEPRECATED)
**gi_taxid_prot_diff.dmp** | [NCBI][gi_taxid] | Differences between this and previous gi_taxid_prot.dmp (DEPRECATED)


The databases available within
`/sw/data/uppnex/ncbi_taxonomy/latest/accession2taxid` are below.  The
**dead_** files contain accession-to-TaxID mappings for dead (suppressed or
withdrawn) sequence records.  For more on each, see the links.

**Name** | **Source** | **Notes**
-----|------|--------
**nucl_est.accession2taxid** | [NCBI][acc2tax] | TaxID mapping for nucleotide records of type EST
**nucl_gss.accession2taxid** | [NCBI][acc2tax] | TaxID mapping for nucleotide records of type GSS
**nucl_wgs.accession2taxid** | [NCBI][acc2tax] | TaxID mapping for nucleotide records of type WGS or TSA
**nucl_gb.accession2taxid** | [NCBI][acc2tax] | TaxID mapping for nucleotide records not of the above types
**prot.accession2taxid** | [NCBI][acc2tax] | TaxID mapping for protein records
**pdb.accession2taxid** | [NCBI][acc2tax] | TaxID mapping for PDB protein records
**dead_nucl.accession2taxid** | [NCBI][acc2tax] | TaxID mapping for dead nucleotide records
**dead_prot.accession2taxid** | [NCBI][acc2tax] | TaxID mapping for dead protein records
**dead_wgs.accession2taxid** | [NCBI][acc2tax] | TaxID mapping for dead WGS or TSA records


The **biocollections** databases contain collections location information.
`coll_dump.txt` is located within the `/sw/data/uppnex/ncbi_taxonomy/latest`
directory.  Those marked **biocollections** are located within the
`/sw/data/uppnex/ncbi_taxonomy/latest/biocollections` directory.

**Name** | **Source** | **Notes**
-----|------|-----
**coll_dump.txt** | [NCBI][taxonomy] | 
**Collection_codes.txt** | [NCBI][biocoll] | **biocollections**
**Institution_codes.txt** | [NCBI][biocoll] | **biocollections**
**Unique_institution_codes.txt** | [NCBI][biocoll] | **biocollections**


[taxdump]:  ftp://ftp.ncbi.nlm.nih.gov/pub/taxonomy/taxdump_readme.txt
[taxcat]:   ftp://ftp.ncbi.nlm.nih.gov/pub/taxonomy/taxcat_readme.txt
[gi_taxid]: ftp://ftp.ncbi.nlm.nih.gov/pub/taxonomy/gi_taxid.readme
[acc2tax]:  ftp://ftp.ncbi.nlm.nih.gov/pub/taxonomy/accession2taxid/README
[taxonomy]: ftp://ftp.ncbi.nlm.nih.gov/pub/taxonomy
[biocoll]:  ftp://ftp.ncbi.nlm.nih.gov/pub/taxonomy/biocollections

