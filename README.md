# Linux_Lwip
Steps to run LWIP on Linux
   1. Download the latest Contrib and lwip from http://nongnu.askapache.com/lwip/
   2. Keep both in same folder/directory 
   3. Rename the lwip-xxxxx contain sources directory to lwip
   4. Copy the lwipopts.h from contrib-x.x.x/examples/example_app/lwipopts.h  lwip/src/include/lwipopts.h 
          - lwipopts provides the option to enable/disaple features and module-debug support 
   5. Rename the Contrib-x.x.x/examples/example_app/lwipcfg.h.example to Contrib-x.x.x/examples/example_app/lwipcfg.h
   6. Go to contrib-x.x.x/ports/unix/example_app (cd contrib-x.x.x/ports/unix/example_app)
   7. Create build directory(mkdir build)
   8. cd build
   9. cmake ..
   10. make clean all
   11. Sample linux based executable example_app avilable at contrib-x.x.x/ports/unix/example_app/build
