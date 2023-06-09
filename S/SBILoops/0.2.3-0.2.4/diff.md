# Comparing `tmp/SBILoops-0.2.3.tar.gz` & `tmp/SBILoops-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SBILoops-0.2.3.tar", last modified: Thu Jun  8 19:03:31 2023, max compression
+gzip compressed data, was "SBILoops-0.2.4.tar", last modified: Fri Jun  9 14:49:41 2023, max compression
```

## Comparing `SBILoops-0.2.3.tar` & `SBILoops-0.2.4.tar`

### file list

```diff
@@ -1,152 +1,155 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.322044 SBILoops-0.2.3/
--rw-r--r--   0 patrick    (501) staff       (20)    24218 2023-06-08 19:03:31.322290 SBILoops-0.2.3/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)    23955 2023-06-05 22:00:16.000000 SBILoops-0.2.3/README.md
--rw-r--r--   0 patrick    (501) staff       (20)      102 2023-06-08 19:03:31.323044 SBILoops-0.2.3/setup.cfg
--rw-r--r--   0 patrick    (501) staff       (20)      589 2023-06-08 19:02:33.000000 SBILoops-0.2.3/setup.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.060380 SBILoops-0.2.3/src/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.077103 SBILoops-0.2.3/src/SBILoops/
--rw-r--r--   0 patrick    (501) staff       (20)    12913 2023-06-08 19:02:11.000000 SBILoops-0.2.3/src/SBILoops/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.103358 SBILoops-0.2.3/src/SBILoops/beans/
--rw-r--r--   0 patrick    (501) staff       (20)     4502 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/beans/Executable.py
--rw-r--r--   0 patrick    (501) staff       (20)    11705 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/beans/File.py
--rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/beans/IndexedNum.py
--rw-r--r--   0 patrick    (501) staff       (20)      349 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/beans/JSONer.py
--rw-r--r--   0 patrick    (501) staff       (20)    14934 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/beans/Path.py
--rw-r--r--   0 patrick    (501) staff       (20)     2928 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/beans/StorableObject.py
--rw-r--r--   0 patrick    (501) staff       (20)      187 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/beans/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-06-05 19:37:25.000000 SBILoops-0.2.3/src/SBILoops/beans/butler.py
--rw-r--r--   0 patrick    (501) staff       (20)      516 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/beans/singleton.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.117301 SBILoops-0.2.3/src/SBILoops/data/
--rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/data/Alphabet.py
--rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/data/AminoAcids.py
--rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/data/AtomVariants.py
--rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/data/Element.py
--rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/data/Properties.py
--rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/data/SetDict.py
--rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/data/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.147354 SBILoops-0.2.3/src/SBILoops/databases/
--rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/databases/CATHlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     8418 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/databases/DrugBanklink.py
--rw-r--r--   0 patrick    (501) staff       (20)    13623 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/databases/Enzymelink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5579 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/databases/GOlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5361 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/databases/PDBTMlink.py
--rw-r--r--   0 patrick    (501) staff       (20)      417 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/databases/PDBeChemConnect.py
--rw-r--r--   0 patrick    (501) staff       (20)     6723 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/databases/PDBeChemlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     9135 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/databases/PDBlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     1801 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/databases/SCOPlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5741 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/databases/TaxIDlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7108 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/databases/Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7073 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/databases/__Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/databases/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     7155 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/databases/dblink.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.153055 SBILoops-0.2.3/src/SBILoops/databases/uniprot/
--rw-r--r--   0 patrick    (501) staff       (20)       90 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/databases/uniprot/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     4783 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/databases/uniprot/connect.py
--rw-r--r--   0 patrick    (501) staff       (20)     8173 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/databases/uniprot/uniprot.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.161617 SBILoops-0.2.3/src/SBILoops/error/
--rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/error/BlastError.py
--rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/error/FileError.py
--rw-r--r--   0 patrick    (501) staff       (20)      896 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/error/SeqAliError.py
--rw-r--r--   0 patrick    (501) staff       (20)      108 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/error/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.164286 SBILoops-0.2.3/src/SBILoops/external/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.172579 SBILoops-0.2.3/src/SBILoops/external/CDhit/
--rw-r--r--   0 patrick    (501) staff       (20)      964 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/external/CDhit/CDhit.py
--rw-r--r--   0 patrick    (501) staff       (20)     2261 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/external/CDhit/CDhitExe.py
--rw-r--r--   0 patrick    (501) staff       (20)      802 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/external/CDhit/CDhitHomolog.py
--rw-r--r--   0 patrick    (501) staff       (20)     2227 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/external/CDhit/CDhitList.py
--rw-r--r--   0 patrick    (501) staff       (20)       64 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/external/CDhit/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.179387 SBILoops-0.2.3/src/SBILoops/external/DSSP/
--rw-r--r--   0 patrick    (501) staff       (20)     3326 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/external/DSSP/DSSP.py
--rw-r--r--   0 patrick    (501) staff       (20)     3608 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/external/DSSP/DSSPExe.py
--rw-r--r--   0 patrick    (501) staff       (20)       54 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/external/DSSP/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)       62 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/external/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.190204 SBILoops-0.2.3/src/SBILoops/external/blast/
--rw-r--r--   0 patrick    (501) staff       (20)     9121 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/external/blast/BlastExe.py
--rw-r--r--   0 patrick    (501) staff       (20)    12572 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/external/blast/BlastHit.py
--rw-r--r--   0 patrick    (501) staff       (20)    23494 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/external/blast/BlastResult.py
--rw-r--r--   0 patrick    (501) staff       (20)       83 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/external/blast/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     8076 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/external/blast/blast_parser.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.193321 SBILoops-0.2.3/src/SBILoops/math/
--rw-r--r--   0 patrick    (501) staff       (20)       19 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/math/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/math/stats.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.204158 SBILoops-0.2.3/src/SBILoops/sequence/
--rw-r--r--   0 patrick    (501) staff       (20)     6337 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/sequence/Fasta.py
--rw-r--r--   0 patrick    (501) staff       (20)     4877 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/sequence/IndexedSeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)    15049 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/sequence/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/sequence/Sequence.py
--rw-r--r--   0 patrick    (501) staff       (20)      140 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/sequence/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.214783 SBILoops-0.2.3/src/SBILoops/sequence/alignment/
--rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/sequence/alignment/Needleman_Wunsch.py
--rw-r--r--   0 patrick    (501) staff       (20)    43530 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/sequence/alignment/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/sequence/alignment/SimilarityMatrix.py
--rw-r--r--   0 patrick    (501) staff       (20)       93 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/sequence/alignment/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.223677 SBILoops-0.2.3/src/SBILoops/structure/
--rw-r--r--   0 patrick    (501) staff       (20)    20850 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/PDB.py
--rw-r--r--   0 patrick    (501) staff       (20)      460 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.233479 SBILoops-0.2.3/src/SBILoops/structure/atom/
--rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/atom/Atom.py
--rw-r--r--   0 patrick    (501) staff       (20)      659 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/atom/AtomOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)      803 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/atom/AtomOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     3764 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/atom/AtomSeries.py
--rw-r--r--   0 patrick    (501) staff       (20)      127 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/atom/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.244362 SBILoops-0.2.3/src/SBILoops/structure/chain/
--rw-r--r--   0 patrick    (501) staff       (20)    19968 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/chain/Chain.py
--rw-r--r--   0 patrick    (501) staff       (20)    13270 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/chain/ChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)     2765 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/chain/ChainOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     6879 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/chain/ChainOfProtein.py
--rw-r--r--   0 patrick    (501) staff       (20)     4992 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/chain/ProteinChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)      131 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/chain/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.249992 SBILoops-0.2.3/src/SBILoops/structure/contacts/
--rw-r--r--   0 patrick    (501) staff       (20)     9012 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/Complex.py
--rw-r--r--   0 patrick    (501) staff       (20)     3410 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/InnerContacts.py
--rw-r--r--   0 patrick    (501) staff       (20)      277 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.258859 SBILoops-0.2.3/src/SBILoops/structure/contacts/contact/
--rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/contact/Contact.py
--rw-r--r--   0 patrick    (501) staff       (20)     3808 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/contact/ContactAA.py
--rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/contact/ContactAH.py
--rw-r--r--   0 patrick    (501) staff       (20)     3277 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/contact/ContactAN.py
--rw-r--r--   0 patrick    (501) staff       (20)      149 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/contact/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.265639 SBILoops-0.2.3/src/SBILoops/structure/contacts/inner/
--rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/inner/PHInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/inner/PPInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)       85 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/inner/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.273543 SBILoops-0.2.3/src/SBILoops/structure/contacts/interface/
--rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/interface/Interface.py
--rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/interface/PHInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    11117 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/interface/PNInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/interface/PPInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)      157 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/contacts/interface/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.278531 SBILoops-0.2.3/src/SBILoops/structure/geometry/
--rw-r--r--   0 patrick    (501) staff       (20)    11106 2023-06-08 18:06:09.000000 SBILoops-0.2.3/src/SBILoops/structure/geometry/RMSD.py
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-06-08 18:05:00.000000 SBILoops-0.2.3/src/SBILoops/structure/geometry/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      662 2023-06-08 18:05:43.000000 SBILoops-0.2.3/src/SBILoops/structure/geometry/basics.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.298967 SBILoops-0.2.3/src/SBILoops/structure/header/
--rw-r--r--   0 patrick    (501) staff       (20)     2284 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/header/BioMolecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     3831 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/header/DBreference.py
--rw-r--r--   0 patrick    (501) staff       (20)     2015 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/header/Experiment.py
--rw-r--r--   0 patrick    (501) staff       (20)    14756 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/header/Header.py
--rw-r--r--   0 patrick    (501) staff       (20)     1201 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/header/HeteroAtom.py
--rw-r--r--   0 patrick    (501) staff       (20)      948 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/header/MiniRes.py
--rw-r--r--   0 patrick    (501) staff       (20)     7647 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/header/Molecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     8534 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/header/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     2423 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/header/Site.py
--rw-r--r--   0 patrick    (501) staff       (20)    18695 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/header/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    14370 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/parse_mmCIF.py
--rw-r--r--   0 patrick    (501) staff       (20)     8543 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/parse_pdb.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.311442 SBILoops-0.2.3/src/SBILoops/structure/protein/
--rw-r--r--   0 patrick    (501) staff       (20)    19074 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/protein/Arch.py
--rw-r--r--   0 patrick    (501) staff       (20)    19202 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/protein/SShelper.py
--rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/protein/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/protein/Sequencer.py
--rw-r--r--   0 patrick    (501) staff       (20)      134 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/protein/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.320579 SBILoops-0.2.3/src/SBILoops/structure/residue/
--rw-r--r--   0 patrick    (501) staff       (20)    10773 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/residue/Residue.py
--rw-r--r--   0 patrick    (501) staff       (20)    10725 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/residue/ResidueOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)     5359 2023-06-05 21:34:52.000000 SBILoops-0.2.3/src/SBILoops/structure/residue/ResidueOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)      146 2023-06-05 17:30:37.000000 SBILoops-0.2.3/src/SBILoops/structure/residue/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-08 19:03:31.084500 SBILoops-0.2.3/src/SBILoops.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)    24218 2023-06-08 19:03:31.000000 SBILoops-0.2.3/src/SBILoops.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     4901 2023-06-08 19:03:31.000000 SBILoops-0.2.3/src/SBILoops.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-06-08 19:03:31.000000 SBILoops-0.2.3/src/SBILoops.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)       39 2023-06-08 19:03:31.000000 SBILoops-0.2.3/src/SBILoops.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)        9 2023-06-08 19:03:31.000000 SBILoops-0.2.3/src/SBILoops.egg-info/top_level.txt
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.654126 SBILoops-0.2.4/
+-rw-r--r--   0 patrick    (501) staff       (20)       84 2023-06-08 19:32:47.000000 SBILoops-0.2.4/MANIFEST.in
+-rw-r--r--   0 patrick    (501) staff       (20)    24218 2023-06-09 14:49:41.655758 SBILoops-0.2.4/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)    23955 2023-06-05 22:00:16.000000 SBILoops-0.2.4/README.md
+-rw-r--r--   0 patrick    (501) staff       (20)      102 2023-06-09 14:49:41.657232 SBILoops-0.2.4/setup.cfg
+-rw-r--r--   0 patrick    (501) staff       (20)      620 2023-06-09 14:48:40.000000 SBILoops-0.2.4/setup.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.337527 SBILoops-0.2.4/src/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.353611 SBILoops-0.2.4/src/SBILoops/
+-rw-r--r--   0 patrick    (501) staff       (20)    12913 2023-06-09 14:49:08.000000 SBILoops-0.2.4/src/SBILoops/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.388864 SBILoops-0.2.4/src/SBILoops/beans/
+-rw-r--r--   0 patrick    (501) staff       (20)     4502 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/beans/Executable.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11705 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/beans/File.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/beans/IndexedNum.py
+-rw-r--r--   0 patrick    (501) staff       (20)      349 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/beans/JSONer.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14934 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/beans/Path.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2928 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/beans/StorableObject.py
+-rw-r--r--   0 patrick    (501) staff       (20)      187 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/beans/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-06-05 19:37:25.000000 SBILoops-0.2.4/src/SBILoops/beans/butler.py
+-rw-r--r--   0 patrick    (501) staff       (20)      516 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/beans/singleton.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.406319 SBILoops-0.2.4/src/SBILoops/data/
+-rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/data/Alphabet.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/data/AminoAcids.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/data/AtomVariants.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/data/Element.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/data/Properties.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/data/SetDict.py
+-rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/data/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.439023 SBILoops-0.2.4/src/SBILoops/databases/
+-rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/databases/CATHlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8418 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/databases/DrugBanklink.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13623 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/databases/Enzymelink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5579 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/databases/GOlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5361 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/databases/PDBTMlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)      417 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/databases/PDBeChemConnect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6723 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/databases/PDBeChemlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9135 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/databases/PDBlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1801 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/databases/SCOPlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5741 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/databases/TaxIDlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7108 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/databases/Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7073 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/databases/__Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/databases/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7155 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/databases/dblink.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.447919 SBILoops-0.2.4/src/SBILoops/databases/uniprot/
+-rw-r--r--   0 patrick    (501) staff       (20)       90 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/databases/uniprot/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4783 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/databases/uniprot/connect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8173 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/databases/uniprot/uniprot.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.460988 SBILoops-0.2.4/src/SBILoops/error/
+-rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/error/BlastError.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/error/FileError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      896 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/error/SeqAliError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      108 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/error/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.466307 SBILoops-0.2.4/src/SBILoops/external/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.478007 SBILoops-0.2.4/src/SBILoops/external/CDhit/
+-rw-r--r--   0 patrick    (501) staff       (20)      964 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/external/CDhit/CDhit.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2261 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/external/CDhit/CDhitExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)      802 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/external/CDhit/CDhitHomolog.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2227 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/external/CDhit/CDhitList.py
+-rw-r--r--   0 patrick    (501) staff       (20)       64 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/external/CDhit/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.485038 SBILoops-0.2.4/src/SBILoops/external/DSSP/
+-rw-r--r--   0 patrick    (501) staff       (20)     3326 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/external/DSSP/DSSP.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3608 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/external/DSSP/DSSPExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)       54 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/external/DSSP/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      338 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/external/README.md
+-rw-r--r--   0 patrick    (501) staff       (20)       62 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/external/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.495967 SBILoops-0.2.4/src/SBILoops/external/blast/
+-rw-r--r--   0 patrick    (501) staff       (20)     9121 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/external/blast/BlastExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12572 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/external/blast/BlastHit.py
+-rw-r--r--   0 patrick    (501) staff       (20)    23494 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/external/blast/BlastResult.py
+-rw-r--r--   0 patrick    (501) staff       (20)       83 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/external/blast/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8076 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/external/blast/blast_parser.py
+-rw-r--r--   0 patrick    (501) staff       (20)      312 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/external/configSBI.txt
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.500154 SBILoops-0.2.4/src/SBILoops/math/
+-rw-r--r--   0 patrick    (501) staff       (20)       19 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/math/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/math/stats.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.512805 SBILoops-0.2.4/src/SBILoops/sequence/
+-rw-r--r--   0 patrick    (501) staff       (20)     6337 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/sequence/Fasta.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4877 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/sequence/IndexedSeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)    15049 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/sequence/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/sequence/Sequence.py
+-rw-r--r--   0 patrick    (501) staff       (20)      140 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/sequence/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.523406 SBILoops-0.2.4/src/SBILoops/sequence/alignment/
+-rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/sequence/alignment/Needleman_Wunsch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    43530 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/sequence/alignment/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/sequence/alignment/SimilarityMatrix.py
+-rw-r--r--   0 patrick    (501) staff       (20)       93 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/sequence/alignment/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.534322 SBILoops-0.2.4/src/SBILoops/structure/
+-rw-r--r--   0 patrick    (501) staff       (20)    20850 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/PDB.py
+-rw-r--r--   0 patrick    (501) staff       (20)      460 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.545347 SBILoops-0.2.4/src/SBILoops/structure/atom/
+-rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/atom/Atom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      659 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/atom/AtomOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)      803 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/atom/AtomOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3764 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/atom/AtomSeries.py
+-rw-r--r--   0 patrick    (501) staff       (20)      127 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/atom/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.558688 SBILoops-0.2.4/src/SBILoops/structure/chain/
+-rw-r--r--   0 patrick    (501) staff       (20)    19968 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/chain/Chain.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13270 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/chain/ChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2765 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/chain/ChainOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6879 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/chain/ChainOfProtein.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4992 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/chain/ProteinChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)      131 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/chain/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.565079 SBILoops-0.2.4/src/SBILoops/structure/contacts/
+-rw-r--r--   0 patrick    (501) staff       (20)     9012 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/Complex.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3410 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/InnerContacts.py
+-rw-r--r--   0 patrick    (501) staff       (20)      277 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.577299 SBILoops-0.2.4/src/SBILoops/structure/contacts/contact/
+-rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/contact/Contact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3808 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/contact/ContactAA.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/contact/ContactAH.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3277 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/contact/ContactAN.py
+-rw-r--r--   0 patrick    (501) staff       (20)      149 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/contact/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.583716 SBILoops-0.2.4/src/SBILoops/structure/contacts/inner/
+-rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/inner/PHInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/inner/PPInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)       85 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/inner/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.597173 SBILoops-0.2.4/src/SBILoops/structure/contacts/interface/
+-rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/interface/Interface.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/interface/PHInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11117 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/interface/PNInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/interface/PPInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)      157 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/contacts/interface/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.602830 SBILoops-0.2.4/src/SBILoops/structure/geometry/
+-rw-r--r--   0 patrick    (501) staff       (20)    11106 2023-06-08 18:06:09.000000 SBILoops-0.2.4/src/SBILoops/structure/geometry/RMSD.py
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-06-08 18:05:00.000000 SBILoops-0.2.4/src/SBILoops/structure/geometry/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      662 2023-06-08 18:05:43.000000 SBILoops-0.2.4/src/SBILoops/structure/geometry/basics.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.628151 SBILoops-0.2.4/src/SBILoops/structure/header/
+-rw-r--r--   0 patrick    (501) staff       (20)     2284 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/header/BioMolecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3831 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/header/DBreference.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2015 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/header/Experiment.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14756 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/header/Header.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1201 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/header/HeteroAtom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      948 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/header/MiniRes.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7647 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/header/Molecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8534 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/header/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2423 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/header/Site.py
+-rw-r--r--   0 patrick    (501) staff       (20)    18695 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/header/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14370 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/parse_mmCIF.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8543 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/parse_pdb.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.642097 SBILoops-0.2.4/src/SBILoops/structure/protein/
+-rw-r--r--   0 patrick    (501) staff       (20)    19074 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/protein/Arch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    19202 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/protein/SShelper.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/protein/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/protein/Sequencer.py
+-rw-r--r--   0 patrick    (501) staff       (20)      134 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/protein/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.652918 SBILoops-0.2.4/src/SBILoops/structure/residue/
+-rw-r--r--   0 patrick    (501) staff       (20)    10773 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/residue/Residue.py
+-rw-r--r--   0 patrick    (501) staff       (20)    10725 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/residue/ResidueOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5359 2023-06-05 21:34:52.000000 SBILoops-0.2.4/src/SBILoops/structure/residue/ResidueOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)      146 2023-06-05 17:30:37.000000 SBILoops-0.2.4/src/SBILoops/structure/residue/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-06-09 14:49:41.364843 SBILoops-0.2.4/src/SBILoops.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)    24218 2023-06-09 14:49:41.000000 SBILoops-0.2.4/src/SBILoops.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     4981 2023-06-09 14:49:41.000000 SBILoops-0.2.4/src/SBILoops.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-06-09 14:49:41.000000 SBILoops-0.2.4/src/SBILoops.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       39 2023-06-09 14:49:41.000000 SBILoops-0.2.4/src/SBILoops.egg-info/requires.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        9 2023-06-09 14:49:41.000000 SBILoops-0.2.4/src/SBILoops.egg-info/top_level.txt
```

### Comparing `SBILoops-0.2.3/PKG-INFO` & `SBILoops-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SBILoops
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://github.com/structuralbioinformatics/SBI
 Author: Patrick Gohl
 Author-email: patrick.gohl@upf.edu
 License: MIT
 Keywords: Structural Bioinformatics,Loops
 Description-Content-Type: text/markdown
```

### Comparing `SBILoops-0.2.3/README.md` & `SBILoops-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/setup.py` & `SBILoops-0.2.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 with open('README.md') as f:
     readme = f.read()
 
 
 setup(
     name='SBILoops',
-    version='0.2.3',
+    version='0.2.4',
     license='MIT',
     author="Patrick Gohl",
     author_email='patrick.gohl@upf.edu',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
+    include_package_data=True,
     long_description=readme,
     long_description_content_type="text/markdown",
     url='https://github.com/structuralbioinformatics/SBI',
     keywords='Structural Bioinformatics, Loops',
     install_requires=[
           'numpy','pandas','pynion','Requests','scipy','six'
       ],
```

### Comparing `SBILoops-0.2.3/src/SBILoops/__init__.py` & `SBILoops-0.2.4/src/SBILoops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sys
 import os
 import traceback
 import datetime
 import time
 import logging
 
-__version__ = '0.2.3'
+__version__ = '0.2.4'
 
 
 class Parameters(object):
     '''
     Designed to work through all the {SBI} library.
     It contains several parameters that will control (a) the amount of data
     shown to the user during the execution of {SBI} subroutines and (b) the
```

### Comparing `SBILoops-0.2.3/src/SBILoops/beans/Executable.py` & `SBILoops-0.2.4/src/SBILoops/beans/Executable.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/beans/File.py` & `SBILoops-0.2.4/src/SBILoops/beans/File.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/beans/IndexedNum.py` & `SBILoops-0.2.4/src/SBILoops/beans/IndexedNum.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/beans/Path.py` & `SBILoops-0.2.4/src/SBILoops/beans/Path.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/beans/StorableObject.py` & `SBILoops-0.2.4/src/SBILoops/beans/StorableObject.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/beans/butler.py` & `SBILoops-0.2.4/src/SBILoops/beans/butler.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/beans/singleton.py` & `SBILoops-0.2.4/src/SBILoops/beans/singleton.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/data/Alphabet.py` & `SBILoops-0.2.4/src/SBILoops/data/Alphabet.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/data/AminoAcids.py` & `SBILoops-0.2.4/src/SBILoops/data/AminoAcids.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/data/AtomVariants.py` & `SBILoops-0.2.4/src/SBILoops/data/AtomVariants.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/data/Element.py` & `SBILoops-0.2.4/src/SBILoops/data/Element.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/data/Properties.py` & `SBILoops-0.2.4/src/SBILoops/data/Properties.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/data/SetDict.py` & `SBILoops-0.2.4/src/SBILoops/data/SetDict.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/data/__init__.py` & `SBILoops-0.2.4/src/SBILoops/data/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/databases/CATHlink.py` & `SBILoops-0.2.4/src/SBILoops/databases/CATHlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/databases/DrugBanklink.py` & `SBILoops-0.2.4/src/SBILoops/databases/DrugBanklink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/databases/Enzymelink.py` & `SBILoops-0.2.4/src/SBILoops/databases/Enzymelink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/databases/GOlink.py` & `SBILoops-0.2.4/src/SBILoops/databases/GOlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/databases/PDBTMlink.py` & `SBILoops-0.2.4/src/SBILoops/databases/PDBTMlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/databases/PDBeChemlink.py` & `SBILoops-0.2.4/src/SBILoops/databases/PDBeChemlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/databases/PDBlink.py` & `SBILoops-0.2.4/src/SBILoops/databases/PDBlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/databases/SCOPlink.py` & `SBILoops-0.2.4/src/SBILoops/databases/SCOPlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/databases/TaxIDlink.py` & `SBILoops-0.2.4/src/SBILoops/databases/TaxIDlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/databases/Uniprotlink.py` & `SBILoops-0.2.4/src/SBILoops/databases/Uniprotlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/databases/__Uniprotlink.py` & `SBILoops-0.2.4/src/SBILoops/databases/__Uniprotlink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/databases/__init__.py` & `SBILoops-0.2.4/src/SBILoops/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/databases/dblink.py` & `SBILoops-0.2.4/src/SBILoops/databases/dblink.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/databases/uniprot/connect.py` & `SBILoops-0.2.4/src/SBILoops/databases/uniprot/connect.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/databases/uniprot/uniprot.py` & `SBILoops-0.2.4/src/SBILoops/databases/uniprot/uniprot.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/error/BlastError.py` & `SBILoops-0.2.4/src/SBILoops/error/BlastError.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/error/FileError.py` & `SBILoops-0.2.4/src/SBILoops/error/FileError.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/error/SeqAliError.py` & `SBILoops-0.2.4/src/SBILoops/error/SeqAliError.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/external/CDhit/CDhit.py` & `SBILoops-0.2.4/src/SBILoops/external/CDhit/CDhit.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/external/CDhit/CDhitExe.py` & `SBILoops-0.2.4/src/SBILoops/external/CDhit/CDhitExe.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/external/CDhit/CDhitHomolog.py` & `SBILoops-0.2.4/src/SBILoops/external/CDhit/CDhitHomolog.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/external/CDhit/CDhitList.py` & `SBILoops-0.2.4/src/SBILoops/external/CDhit/CDhitList.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/external/DSSP/DSSP.py` & `SBILoops-0.2.4/src/SBILoops/external/DSSP/DSSP.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/external/DSSP/DSSPExe.py` & `SBILoops-0.2.4/src/SBILoops/external/DSSP/DSSPExe.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/external/blast/BlastExe.py` & `SBILoops-0.2.4/src/SBILoops/external/blast/BlastExe.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/external/blast/BlastHit.py` & `SBILoops-0.2.4/src/SBILoops/external/blast/BlastHit.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/external/blast/BlastResult.py` & `SBILoops-0.2.4/src/SBILoops/external/blast/BlastResult.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/external/blast/blast_parser.py` & `SBILoops-0.2.4/src/SBILoops/external/blast/blast_parser.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/math/stats.py` & `SBILoops-0.2.4/src/SBILoops/math/stats.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/sequence/Fasta.py` & `SBILoops-0.2.4/src/SBILoops/sequence/Fasta.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/sequence/IndexedSeqAli.py` & `SBILoops-0.2.4/src/SBILoops/sequence/IndexedSeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/sequence/SeqAli.py` & `SBILoops-0.2.4/src/SBILoops/sequence/SeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/sequence/Sequence.py` & `SBILoops-0.2.4/src/SBILoops/sequence/Sequence.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/sequence/alignment/Needleman_Wunsch.py` & `SBILoops-0.2.4/src/SBILoops/sequence/alignment/Needleman_Wunsch.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/sequence/alignment/SeqAli.py` & `SBILoops-0.2.4/src/SBILoops/sequence/alignment/SeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/sequence/alignment/SimilarityMatrix.py` & `SBILoops-0.2.4/src/SBILoops/sequence/alignment/SimilarityMatrix.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/PDB.py` & `SBILoops-0.2.4/src/SBILoops/structure/PDB.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/atom/Atom.py` & `SBILoops-0.2.4/src/SBILoops/structure/atom/Atom.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/atom/AtomOfAminoAcid.py` & `SBILoops-0.2.4/src/SBILoops/structure/atom/AtomOfAminoAcid.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/atom/AtomOfNucleotide.py` & `SBILoops-0.2.4/src/SBILoops/structure/atom/AtomOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/atom/AtomSeries.py` & `SBILoops-0.2.4/src/SBILoops/structure/atom/AtomSeries.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/chain/Chain.py` & `SBILoops-0.2.4/src/SBILoops/structure/chain/Chain.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/chain/ChainFrame.py` & `SBILoops-0.2.4/src/SBILoops/structure/chain/ChainFrame.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/chain/ChainOfNucleotide.py` & `SBILoops-0.2.4/src/SBILoops/structure/chain/ChainOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/chain/ChainOfProtein.py` & `SBILoops-0.2.4/src/SBILoops/structure/chain/ChainOfProtein.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/chain/ProteinChainFrame.py` & `SBILoops-0.2.4/src/SBILoops/structure/chain/ProteinChainFrame.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/contacts/Complex.py` & `SBILoops-0.2.4/src/SBILoops/structure/contacts/Complex.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/contacts/InnerContacts.py` & `SBILoops-0.2.4/src/SBILoops/structure/contacts/InnerContacts.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/contacts/contact/Contact.py` & `SBILoops-0.2.4/src/SBILoops/structure/contacts/contact/Contact.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/contacts/contact/ContactAA.py` & `SBILoops-0.2.4/src/SBILoops/structure/contacts/contact/ContactAA.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/contacts/contact/ContactAH.py` & `SBILoops-0.2.4/src/SBILoops/structure/contacts/contact/ContactAH.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/contacts/contact/ContactAN.py` & `SBILoops-0.2.4/src/SBILoops/structure/contacts/contact/ContactAN.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/contacts/inner/PHInnerContact.py` & `SBILoops-0.2.4/src/SBILoops/structure/contacts/inner/PHInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/contacts/inner/PPInnerContact.py` & `SBILoops-0.2.4/src/SBILoops/structure/contacts/inner/PPInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/contacts/interface/Interface.py` & `SBILoops-0.2.4/src/SBILoops/structure/contacts/interface/Interface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/contacts/interface/PHInterface.py` & `SBILoops-0.2.4/src/SBILoops/structure/contacts/interface/PHInterface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/contacts/interface/PNInterface.py` & `SBILoops-0.2.4/src/SBILoops/structure/contacts/interface/PNInterface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/contacts/interface/PPInterface.py` & `SBILoops-0.2.4/src/SBILoops/structure/contacts/interface/PPInterface.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/geometry/RMSD.py` & `SBILoops-0.2.4/src/SBILoops/structure/geometry/RMSD.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/geometry/basics.py` & `SBILoops-0.2.4/src/SBILoops/structure/geometry/basics.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/header/BioMolecule.py` & `SBILoops-0.2.4/src/SBILoops/structure/header/BioMolecule.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/header/DBreference.py` & `SBILoops-0.2.4/src/SBILoops/structure/header/DBreference.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/header/Experiment.py` & `SBILoops-0.2.4/src/SBILoops/structure/header/Experiment.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/header/Header.py` & `SBILoops-0.2.4/src/SBILoops/structure/header/Header.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/header/HeteroAtom.py` & `SBILoops-0.2.4/src/SBILoops/structure/header/HeteroAtom.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/header/MiniRes.py` & `SBILoops-0.2.4/src/SBILoops/structure/header/MiniRes.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/header/Molecule.py` & `SBILoops-0.2.4/src/SBILoops/structure/header/Molecule.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/header/SecondaryStructure.py` & `SBILoops-0.2.4/src/SBILoops/structure/header/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/header/Site.py` & `SBILoops-0.2.4/src/SBILoops/structure/header/Site.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/header/__init__.py` & `SBILoops-0.2.4/src/SBILoops/structure/header/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/parse_mmCIF.py` & `SBILoops-0.2.4/src/SBILoops/structure/parse_mmCIF.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/parse_pdb.py` & `SBILoops-0.2.4/src/SBILoops/structure/parse_pdb.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/protein/Arch.py` & `SBILoops-0.2.4/src/SBILoops/structure/protein/Arch.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/protein/SShelper.py` & `SBILoops-0.2.4/src/SBILoops/structure/protein/SShelper.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/protein/SecondaryStructure.py` & `SBILoops-0.2.4/src/SBILoops/structure/protein/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/protein/Sequencer.py` & `SBILoops-0.2.4/src/SBILoops/structure/protein/Sequencer.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/residue/Residue.py` & `SBILoops-0.2.4/src/SBILoops/structure/residue/Residue.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/residue/ResidueOfAminoAcid.py` & `SBILoops-0.2.4/src/SBILoops/structure/residue/ResidueOfAminoAcid.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops/structure/residue/ResidueOfNucleotide.py` & `SBILoops-0.2.4/src/SBILoops/structure/residue/ResidueOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILoops-0.2.3/src/SBILoops.egg-info/PKG-INFO` & `SBILoops-0.2.4/src/SBILoops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SBILoops
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://github.com/structuralbioinformatics/SBI
 Author: Patrick Gohl
 Author-email: patrick.gohl@upf.edu
 License: MIT
 Keywords: Structural Bioinformatics,Loops
 Description-Content-Type: text/markdown
```

### Comparing `SBILoops-0.2.3/src/SBILoops.egg-info/SOURCES.txt` & `SBILoops-0.2.4/src/SBILoops.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+MANIFEST.in
 README.md
 setup.cfg
 setup.py
 src/SBILoops/__init__.py
 src/SBILoops.egg-info/PKG-INFO
 src/SBILoops.egg-info/SOURCES.txt
 src/SBILoops.egg-info/dependency_links.txt
@@ -40,15 +41,17 @@
 src/SBILoops/databases/uniprot/__init__.py
 src/SBILoops/databases/uniprot/connect.py
 src/SBILoops/databases/uniprot/uniprot.py
 src/SBILoops/error/BlastError.py
 src/SBILoops/error/FileError.py
 src/SBILoops/error/SeqAliError.py
 src/SBILoops/error/__init__.py
+src/SBILoops/external/README.md
 src/SBILoops/external/__init__.py
+src/SBILoops/external/configSBI.txt
 src/SBILoops/external/CDhit/CDhit.py
 src/SBILoops/external/CDhit/CDhitExe.py
 src/SBILoops/external/CDhit/CDhitHomolog.py
 src/SBILoops/external/CDhit/CDhitList.py
 src/SBILoops/external/CDhit/__init__.py
 src/SBILoops/external/DSSP/DSSP.py
 src/SBILoops/external/DSSP/DSSPExe.py
```

