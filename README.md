Module Installation Methods
===========================

This is a collection of READMEs generated during installation of software
applications on Uppmax clusters.  It is incomplete in terms of modules
available on Uppmax, and the individual READMEs may also be incomplete in terms
of what was actually done to install the modules.  We are publicising these in
the hopes that they can be helpful.

Scripts
-------

`gather-READMEs.sh` - bash script to scan installation directories, looking for
README files having a particular filename format that we create during
installation of tools

`fixup` - bash script fixing up permissions and group membership within
installation trees; our local installation group is `sw`. With the `-g` option,
this script will `chmod g+s` directories in the tree, too.


Installation directories
------------------------

The directories contain software installations in major subject areas.

### apps/

General applications.

### apps/bioinfo/

Bioinformatics applications.

### libs/

Libraries.

### comp/

Compilers, interpreters, build tools.


Database directories
--------------------

These directories cover installations of databases updated either manually, or via update scripts.

### data_uppnex/

Installation instructions for databases under `/sw/data/uppnex/`.  Database
directories containing `*-install-README.md` files are updated manually.
Database directories containing `*-db-README.md` files and scripts (currently,
`Kraken` and `diamond_databases`) are updated monthly via crontab entries.

### data_other/

Installation instructions for databases under other locations, currently just
`BUSCO` lineage sets, which are kept in the module installation directory.
These are updated monthly via crontab entries.

