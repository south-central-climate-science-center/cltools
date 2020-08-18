Tools to help find netcdf files stored on the climate data server

Example usage:

List the available domains for variable tas:
```findnc variable=tas domain?```

Find and sort netcdf files that meet specific attributes:
```findnc variable=tas domain=day experiment=historical ensemble=r1i1p1 model=inmcm4 | sort```

Copy desired netcdf files to scratch area:
```findnc variable=tas domain=day experiment=historical ensemble=r1i1p1 model=inmcm4 | xargs cp -t /data5/scratch/```
