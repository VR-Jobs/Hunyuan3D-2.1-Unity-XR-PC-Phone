# Hunyuan3D-2.1-Unity-XR-PC-Phone

![新封面](https://github.com/user-attachments/assets/8f1f91fd-94e5-422a-b254-c6e440b3c229)

最近开发了腾讯Hunyuan3D-2.1项目的unity版本！欢迎大家体验！

使用方法
1.新建unity项目，导入glTFast(https://github.com/atteneder/glTFast)
项目。这里采用install package from git url.直接复制链接https://github.com/atteneder/glTFast.git即可

![image](https://github.com/user-attachments/assets/8ac86048-9e3f-49d5-b33a-73b6f99f5a3b)

![image](https://github.com/user-attachments/assets/428d346c-d5a4-475f-8ddc-d58ddb7d013d)

2.导入Newtonsoft Json，这里采用install package by name，复制com.unity.nuget.newtonsoft-json进去即可

![image](https://github.com/user-attachments/assets/d2adfb51-b1d0-49c5-8a24-f9dec2f62e65)

3.解压我们github中的zip文件夹，放到unity的Assets项目里面，然后打开OnGUI场景（服务器Hunyuan3D-OnGUI版本(手机电脑）

![image](https://github.com/user-attachments/assets/f53f731a-9f94-4863-b4ee-fdaaa3dba6bc)

4.观察测试界面

![测试界面](https://github.com/user-attachments/assets/e4cba7d1-a067-4aef-a69d-9453242e46fe)

5.别着急！现在还不能直接使用，还需要上传我们的服务器文件到云服务器里面才可以！首先根据官网配置好云服务器的项目https://github.com/Tencent-Hunyuan/Hunyuan3D-2.1/tree/main

6.配置注意事项：
①注意配置之前，检查自己系统的CUDA情况，python情况，pytorch情况
②注意服务器开放的端口情况，有些服务器只支持个别端口开放
③注意自己服务器性能，这里推荐A100

7.配置完成之后，首先测试gradio程序，直接输入
python gradio_app.py
然后在对应的自己服务器ip地址应该要看到gradio界面，需要确保和huggingface的官网界面相似

![image](https://github.com/user-attachments/assets/57ab72fd-9449-42b8-a2bd-92eec16479ae)

8.上传我们压缩包里面的服务器代码flask_app，到云服务器的项目文件夹下面，确保和gradio_app.py在一个路径下面

![image](https://github.com/user-attachments/assets/e2c09187-05fc-453d-ac17-4b62640b7cc9)
![image](https://github.com/user-attachments/assets/b01ff8bc-b664-47ec-b48f-0554fc53f3e0)


9.先运行服务器测试（以后每次进入都这样输入即可）：
cd ~/Hunyuan3D-2.1
conda activate hunyuan3d-2.1
python flask_app.py

10.成功运行的状态

![image](https://github.com/user-attachments/assets/c08c49c0-8e97-4ae6-a3f7-8aedd6bc2a42)

11.打开unity项目，ongui那个场景，点击运行，就应该看得到左上方有绿灯连接成功

![image](https://github.com/user-attachments/assets/92eb8508-75e0-4e97-8332-7762cc4d2d87)



🔥我也发布了多平台的应用程序，大家可以下载体验Windows版本！手机安卓版本，VR Meta Quest 3版本代码正在整理中

![image](https://github.com/user-attachments/assets/ca1a840a-3701-48f7-826b-25a741cc5852)




