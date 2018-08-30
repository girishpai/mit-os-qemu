# QEMU - Patched for MIT Operating Systems Course (6.828)

Following is the link to the course's tools page which has the instractions to install. 
https://pdos.csail.mit.edu/6.828/2017/tools.html

Unfortunately the link to git repository does not work (git clone hangs). Once you do a git clone of this github repository you can follow the exact same steps. 

Mentioning the steps here for reference (in case the above link breaks in the future). 

I am running on Ubuntu, hence just mentioning the steps for linux. 

1. Configure the source code (optional arguments are shown in square brackets; replace PFX with a path of your choice)
  ./configure --disable-kvm [--prefix=PFX] [--target-list="i386-softmmu x86_64-softmmu"]
  The prefix argument specifies where to install QEMU; without it QEMU will install to /usr/local by default. The target-list argument simply slims down the architectures QEMU will build support for.
  
2. Run make && make install
