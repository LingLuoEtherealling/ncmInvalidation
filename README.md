# NCM Dump
[(Using)](https://github.com/airline12138/ncmdump_php#食用方法)

   [(ncmdump)](https://github.com/SomeBottle/ncm)
   Improvement And Enhancement

## Add
   * [add] Batch dump
   * [fix] Error (lack of ogg3 library introduction)
   * [fix] Flac format cannot write cover image
   * [add] Write song metadata in mp3, flac format
   * [improve] The return mechanism is changed from echo to return, and finally no longer directly output content in the class library
   * [improve] Updated the getid3 class library

## Changelog
   * [fix] Fix the bug that batch dump reports errors and there is no input file
   * [add] Judge whether the input folder exists and does not exist, then exit the execution
   * [add] Judge whether the output folder exists, it will be created automatically if it does not exist

## Extensions needed/functions that need to be turned on/dependent software
   * php_openssl (Decrypt and restore)
   * php_exif (Manipulate image files)

   * shell_exec (getid3 library operation metadata falc)
   * exec (Used to manipulate files)
   * flac (Used to write metadata in flac format 
   * Install in CLI:
   * ( `yum install flac -y` / `apt install flac -y`)

## Class
   * [getID3](https://github.com/JamesHeinrich/getID3)
   * [hex2str](https://www.cnblogs.com/wangluochong/p/11383000.html)
   * [xor](https://www.cnblogs.com/dannywang/p/5316768.html)

## Reference
   * [NCMdump-py](https://github.com/bolitao/ncm)  
   * [ncmdump-php](https://github.com/juzi5201314/ncmdump)

## Using
   单文件dump `php ncm.php <filepath> <dealwithid3>`

   批量dump(All Song) `php dump.php` 需手动修改PHP文件中的`输入NCM路径,输出NCM路径,输出dump后文件路径`(懒得适配CLI)

   [保姆级使用教程](https://blog.qcmoe.com/program/ncmDump.html)

## Thanks
   * [@Jochen233](https://blog.qcmoe.com).
