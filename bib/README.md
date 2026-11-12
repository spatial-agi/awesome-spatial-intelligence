# Bibliography snapshot

`refs.bib` holds the BibTeX entries behind the README: every paper listed, every benchmark row, and every milestone in the historical tables. It is exported from the bibliography of the handbook, so titles, venues and years match the manuscript.

Use it to rebuild the list, to check metadata when adding an entry, or to cite a group of papers at once.

```bash
grep -c "^@" refs.bib
```

The file is a snapshot, not a live mirror. When an entry in the README changes, update it here in the same pull request.
