# Patch By Dalion
由于frida变动较大，用patch的方式修补几乎无法自动成功，使用硬替换的方式，再拉取上游frida后，替换已经手动patch后frida-core 
需要设置Secret PATCH_REPO 为指向frida-core的仓库 如https://github.com/dalion971/frida-core.git
由于替换是硬编码路径不要修改路径及相对路径

```yml
        git clone --recurse-submodules https://github.com/frida/frida
        rm -rf frida/frida-core
        cp -r frida-core frida/frida-core
        cd frida
```

Fork This Repository 


需要设置Secrets
包括
```yml
   GIT_OWNER      
   GIT_REPO
   GIT_CREDENTIALS
   GIT_EMAIL
   GIT_NAME
   PATCH_REPO
```
GIT_CREDENTIALS 在个人github账户开发者设置生成一个



# strongR-frida-android

Follow [FRIDA](https://github.com/frida/frida) upstream to automatic patch and build an anti-detection version of frida-server for android.

跟随 FRIDA 上游自动修补程序，并为 Android 构建反检测版本的 frida-server。

**Hint: Don't fork this repository**

## Patchs

[Git Patch Files](https://github.com/AAAA-Project/Patchs/tree/master/strongR-frida/frida-core)

|module|name|
|-|-|
|frida-core|0001-string_frida_rpc.patch|
|frida-core|0002-io_re_frida_server.patch|
|frida-core|0003-pipe_linjector.patch|
|frida-core|0004-io_frida_agent_so.patch|
|frida-core|0005-symbol_frida_agent_main.patch|
|frida-core|0006-thread_gum_js_loop.patch|
|frida-core|0007-thread_gmain.patch|
|frida-core|0008-protocol_unexpected_command.patch|

## Download

[Latest Release](https://github.com/hzzheyang/strongR-frida-android/releases/latest)

## References

- [https://github.com/feicong/strong-frida](https://github.com/feicong/strong-frida)
- [https://github.com/qtfreet00/AntiFrida](https://github.com/qtfreet00/AntiFrida)
- [https://t.zsxq.com/miIunQN](https://t.zsxq.com/miIunQN)
- [https://github.com/darvincisec/DetectFrida](https://github.com/darvincisec/DetectFrida)
- [https://github.com/b-mueller/frida-detection-demo](https://github.com/b-mueller/frida-detection-demo)

## Thanks

- [@feicong](https://github.com/feicong)
- [@r0ysue](https://github.com/r0ysue)
- [@hellodword](https://github.com/hellodword)
- [@qtfreet00](https://github.com/qtfreet00)

## Discussion

<img src="img/1.png" width = "200" height = "260" alt="" align=center />

## Advert

<img src="img/2.png" width = "180" height = "240" alt="" align=center />

<img src="img/3.png" width = "180" height = "240" alt="" align=center />
