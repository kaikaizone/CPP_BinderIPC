
安卓本地服务框架实例

参考文件:
frameworks\av\include\media\IMediaPlayerService.h     (IMediaPlayerService,BnMediaPlayerService)
frameworks\av\media\libmedia\IMediaPlayerService.cpp                      (BpMediaPlayerService，BnMediaPlayerService类方法的实现)
frameworks\av\media\libmediaplayerservice\MediaPlayerService.h
frameworks\av\media\libmediaplayerservice\MediaPlayerService.cpp （MediaPlayerService::instantiate()添加服务）
frameworks\av\media\mediaserver\Main_mediaserver.cpp   (media_server, addService注册服务 init进程解析rc文件来启动
																		service media /system/bin/mediaserver)
 frameworks\av\media\mediaserver\Android.mk                                                     
 添加到系统：
frameworks/testing/native-service-framework/ 
到此目录仿照mediaserver创建Android.mk文件
执行：mmm编译

Test app for Binder, wrote by C++ language.
=====

compile:  
cd frameworks/testing/native-service-framework/  
   mmm .   
  
####c. run test_server, test_client  
logcat HelloService:* GoodbyeService:* TestService:* *:S &  
./test_server &  
./test_client hello   
./test_client hello   
./test_client hello 
./test_client goodbye  
./test_client goodbye haha 
  
