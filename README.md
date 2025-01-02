# led-blink-test-02
##### 1. if build folder is present in root path of that project.Delete the build folder
##### Cmd: rm -rf build

##### 2. again create build folder and enter the build forlder
##### cmd: mkdir build
##### cmd: cd build 

##### 3. then run the cmake and make cmd:
##### cmd: cmake ..
##### cmd: make 

##### 4. execute the the executable_file
##### cmd:  cd tests/
##### cmd:  ./ledblink_tests


5) To generate the compile_commands.json have to give the command cmake -DCMAKE_EXPORT_COMPILE_COMMANDS=ON ..   within build folder
6) After that if you are running make it will work but test folders has not been enabled to enable give  cmake -DENABLE_TESTS=ON ..
7) make will work to create executables by including tests, 
8)  you can give both the commands cmake -DCMAKE_EXPORT_COMPILE_COMMANDS=ON && cmake -DENABLE_TESTS=ON ..
 
   9)lcov --capture --directory . --output-file /home/purusottam/Downloads/ledblink\ \(1\)/ledblink/build/coverage.info --ignore-errors inconsistent --ignore-errors mismatch

   10)genhtml /home/purusottam/Downloads/ledblink\ \(1\)/ledblink/build/coverage.info --output-directory /home/purusottam/Downloads/ledblink\ \(1\)/ledblink/build/coverage_html --ignore- 
      errors empty
