This is a simple program that plays the role of a Forwarding Plane
Manager and prints out messages received from the RIB. It is useful
for testing the frr code that interacts with the FPM.

*fpm-stub* can be built as follows:

<pre>
  $ make FRR_DIR=&lt;location-of-frr-code&gt;
</pre>

The *FRR\_DIR* variable is required because *fpm\_stub* depends on the
header file that defines the FPM interface (*fpm/fpm.h*).

To run the program, just invoke it as follows -- it will start
listening for a connection from the RIB.

<pre>
  $ ./fpm-stub
</pre>
