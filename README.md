# Samsung-DEX-Standalone-Enable
make sure your device is rooted magisk or kernelsu is fine then download Root Explorer, enable superuser for root explorer in kernelsu or grant superuser request if magisk popup show up, then go to
```
/system/etc
```
mount r/w, edit file called
```
floating_feature.xml
```
find this
```
<SEC_FLOATING_FEATURE_COMMON_CONFIG_DEX_MODE>
```
and look at the value, it should be something like wireless, dual, dexforpc, like this
```
<SEC_FLOATING_FEATURE_COMMON_CONFIG_DEX_MODE>dual,wireless,dexforpc</SEC_FLOATING_FEATURE_COMMON_CONFIG_DEX_MODE>
```
change it into something like this just adding standalone on the value
```
<SEC_FLOATING_FEATURE_COMMON_CONFIG_DEX_MODE>dual,standalone,wireless,dexforpc</SEC_FLOATING_FEATURE_COMMON_CONFIG_DEX_MODE>
```
save the file and reboot your phone now you can use Dex standalone (running dex directly on phone display), tested on S20+, S9, S10e, S10+
