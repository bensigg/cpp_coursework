# cpp_coursework
repo for my alison.com c++ exercises

Started with https://alison.com/course/introduction-to-c-plus-plus-programming as a refresher course.

I made a hello world (hw.cpp) program mostly so I could figure out how I was going to compile and run it.  The course shows usage of Visual Studio, and there exists a Visual Studio for Mac, but it seems to be focused on C#,  I could not figure out how to get it to work on a C++ program, and resorted to command-line g++ instead.

Modules 1 & 2 were mostly things identical with C. They introduced a block syntax for initializing variables I hadn't seen before:
int i{ 4 };
but the g++ command-line compiler doesn't seem to like it.

I spent some time testing the limits of the overloaded operators and indexing operations of the std::string class; see stringtests.cpp.

*** 2 years later ***

Taking on https://alison.com/course/c-plus-plus-programming-advanced-features next.

See basicrefs folder:
Played with some of the sample code from the "references" video of the course.  Doesn't do much, but proves to myself it works the way they said it did.

Learned why I hadn't gotten block initialization `int i{4};` working before - it's part of a later standard than the default used by command-line g++; I have to pass `-std=c++11` or greater.

See inheritance folder:
Copied the Rectangle and NamedRectangle classes off the screen. Wrote sample code that exercised them.

See polymorph folder:
Copied the Triangle class and Shape (its abstract base) class off the screen; minor modifications to Rectangle so it also derives from Shape. Did as the course did, and created a function that takes a Shape reference and appears to call its pure virtual function, which results in the version from the derived class being used.

See raii folder:
Demo used a Squawker class; after understanding its concept, wrote one for myself.  Went beyond the example by adding copy constructor and assignment operator.