I've been fighting all week with configuring uwsgi to work with both
python (wsgi) and ruby (rack) apps.  The python was no problem.
Honestly, the rack stuff wasn't too bad once you sort out the
dependencies.  The real problem I faced was that I manage my rack apps
using bundler, and it is certainly not obvious how to make that work.  I
had actually given up, but then found disturbingly suddent success when
I was waiting for something else to complete.
