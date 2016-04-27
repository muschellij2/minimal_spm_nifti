## Minimal Code from SPM to read/write NIfTI in MATLAB

The code was taken from the [SPM12 package](http://www.fil.ion.ucl.ac.uk/spm/software/spm12/).  

The overall syntax, at least how it's being used in [`matlabr`](https://github.com/muschellij2/matlabr) code is as follows:

```{matlab}
V = spm_vol('filename.nii');
img = spm_read_vols(V);
spm_write_vol(V, img);
```