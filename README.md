

Test app for Binder, wrote by C++ language.
=====

compile:  
cd frameworks/testing/CPP_BinderIPC  
   mmm .   
  
####c. run test_server, test_client  
logcat HelloService:* GoodbyeService:* TestService:* *:S &  
./test_server &  
./test_client hello   
./test_client hello   
./test_client hello 
./test_client goodbye  
./test_client goodbye haha 
  
