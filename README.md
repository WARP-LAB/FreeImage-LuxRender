# FreeImage for LuxRender

This is FreeImage 3.17.0 clone to be used when building LuxRender (on OS X)

* It has general fixes so that it can be compiled with C++11 and -Wc++11-narrowing
* It has altered `Makefile.osx`
	* Builds only 64 bit
	* Specify `MACOSX_DEPLOYMENT_TARGET`
	* For 10.7+ keep `-std=c++11 -stdlib=libc++ -Wc++11-narrowing` in `COMPILERPPFLAGS`
	* For 10.6 change `-std=c++11 -stdlib=libc++ -Wc++11-narrowing` to `-stdlib=libstdc++` in `COMPILERPPFLAGS`
