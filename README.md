

Test app for Binder, wrote by C++ language.
=====

compile:  
--
a. 文件放入frameworks/testing/APP_0004_Binder_CPP_App  
b. cd /work/android-5.0.2/  
   . setenv  
   lunch //选择23. full_tiny4412-eng  
c. cd frameworks/testing/APP_0004_Binder_CPP_App  
   mmm .   
  
####c. run test_server, test_client  
logcat HelloService:* GoodbyeService:* TestService:* *:S &  
./test_server &  
./test_client hello   
./test_client hello   
./test_client hello 
./test_client goodbye  
./test_client goodbye haha 
  
