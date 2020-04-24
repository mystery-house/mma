************************************************
A slight fork of MMA: Musical Midi Accompaniment
************************************************

I wanted to use an MMA function in another project, but I found that the way
the `platform` and `MMApath` variables are derived in `MMA.gbl` assumes that
mma will always be running in its own `__main__` loop, and causes a fatal
error.  I simply moved the declaration of those variables to `MMA/gbl.py` and
that seems to have done the trick.  As far as I know, this code should behave
identically to the official distribution at `<https://www.mellowood.ca/mma/>`_.
