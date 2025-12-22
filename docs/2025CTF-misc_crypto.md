# MISC

## 前置知识

### 语言基础
> 需要学习 python linux  
> 通常使用python编写脚本，如果没有学习过可能无法深入的学习后续的知识  
> 解题会使用linux的一些工具，通常会搭配命令
>

### python 
> 前期学习到函数就够用，导包，变量 数据类型 循环 数组 字典 函数...
>

### linux基础
> 常用命令：
>
> cd ls strings | grep cat file vim mkdir 
>

### 编码 
> base 栅栏 维吉尼亚 凯撒等
>

### 工具
> 010 binwalk foremost zsteg 小鲨鱼 vol等
>

## MISC是什么

### 常见题型
> 隐写 编码转换 zip破解 流量分析
>

### ......

## 常见编码/加密

### 编码
需要记忆常见的编码/加密特征，提高解题速度，一眼顶针

#### base家族
**举例：**

> base16             flag         666C6167  
> base32[A-Z2-7]     flag         MZWGCZY=  
> base36             flag         727432  
> base58             flag         3cr9Ae  
> base64             flag         Zmxh  
> base85             flag         Ao(mg  
> base91             flag         @iH<Z  
> base92             flag         F#S<I  
> base100            flag         👝👣👘👞  
> base2048           flag         ڥڊװ  
> base65535          flag         ꍦ鱡
>

**特征：**

> **Base16编码是将二进制文件转换成由16个字符组成的文本 **
>
> ****
>
> **base32的编码表是由（A-Z、2-7）32个可见字符构成，“=”符号用作后缀填充。**
>
> ****
>
> **base64的编码表是由（A-Z、a-z、0-9、+、/）64个可见字符构成，“=”符号用作后缀填充。**
>
> ****
>
> **base58的编码表相比base64少了数字0，大写字母I，O，小写字母 l (这个是L），以及符号‘+’和‘/’**
>
> ****
>
> **base91的密文由91个字符（0-9，a-z，A-Z,!#$%&()*+,./:;<=>?@[]^_`{|}~”）组成**
>
> ****
>
> **Base100编码/解码工具（又名：Emoji表情符号编码/解码），可将文本内容编码为Emoji表情符号；同时也可以将编码后的Emoji表情符号内容解码为文本。 **
>

常见的熟记，不常见的遇到了可以通过脚本和工具识别解码

#### <font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">ASCII</font>
<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">ASCII 码是对</font>**<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">英语字符与二进制位之间</font>**<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">的关系，做了统一规定。</font>

<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">ASCII 字符集共有 128 个字符，其中有 96 个可打印字符，包括常用的字母、数字、标点符号</font>

**<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">例如：</font>**

<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">数字0为48(二进制：00110000)</font>

<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">大写字母A为65（二进制：01000001）</font>

<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">另外还有32个控制字符（不能打印出来）</font>

<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">这128个符号，只占用了一个字节的后面7位，最前面的一位统一规定为0。</font>

<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);"></font>**<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">特征：</font>**<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);"> </font>**<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">只含有数字</font>**

+ <font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">0-9, 49-57</font>
+ <font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">A-Z, 65-90</font>
+ <font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">a-z, 97-122</font>

**<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">举例：</font>**

> 明文：flag  
> 十六进制：66 6c 61 67  
> 十进制：102 108 97 103  
> 八进制：146 154 141 147  
> 二进制：1100110 1101100 1100001 1100111
>

#### <font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">unicode</font>
> flag: \u0066\u006c\u0061\u0067
>

#### <font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">url</font>
> flag %66%6c%61%67****
>

#### <font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">摩斯电码</font>
> flag  ..-. .-.. .- --.
>

#### <font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">HEX</font>
> flag 666c6167
>

#### <font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">tap code</font>
> flag 21311122
>

最后我们要理解编码和加密的区别

> 编码  
> 目的：编码的主要目的是将数据转换为另一种形式，以便于存储、传输或处理。它确保数据能够在不同的系统或设备之间正确理解和使用。  
> 特点：  
>   ○ 可逆性：编码通常是可逆的，可以通过解码恢复原始数据。  
>   ○ 兼容性：确保数据在不同系统间的兼容性，便于传输和处理。  
> 加密  
> 目的：加密的主要目的是保护数据的机密性和安全性，防止未经授权的访问或篡改。加密数据需要密钥才能解密，确保只有合法用户能够读取数据。  
> 常见加密类型：  
>   ○ 对称加密：使用相同的密钥进行加密和解密，速度快，如AES。  
>   ○ 非对称加密：使用公钥和私钥，如RSA，用于安全通信和数字签名。  
>   ○ 哈希函数：如MD5、SHA-1，生成固定长度的摘要，单向不可逆，常用于数据完整性验证。  
> 特点：  
>   ○ 安全性：加密确保数据在传输或存储中的安全性，防止被窃取或篡改。  
>   ○ 密钥依赖：加密和解密通常需要密钥，只有合法用户才能访问。  
>
> 目的不同：编码用于数据的表示和传输，加密用于数据的安全保护。  
> 可逆性：编码通常是可逆的，而加密需要密钥才能解密，确保数据仅被授权访问。  
> 应用场景：编码常见于数据传输和存储，加密用于保护敏感信息，如密码、支付信息等。
>

### 古典密码

#### 单表
> 单表密码（Monoalphabetic Cipher）是一种最简单的替换密码，通过单一固定的替换表将明文字母映射为密文字母。密钥为替换规则本身，加密过程中每个明文字母始终对应同一密文字母。  
> 示例：凯撒密码（Caesar Cipher）  
> 加密规则：将明文字母向右移动固定位数（如 3 位）
>
> 例如：  
> 明文：A → 密文：D，B → E，…，Z → C。  
> 密钥：移动位数（如 3）。  
> 特点：替换规则固定，同一明文字母始终生成相同密文字母。
>

#### 多表
> 多表密码（Polyalphabetic Cipher）使用多个替换表，根据密钥动态选择不同的替换规则，同一明文字母在不同位置可能被替换为不同密文字母。  
> 示例：维吉尼亚密码（Vigenère Cipher）  
> 加密规则：以密钥短语（如 “KEY”）为周期，每个明文字母根据密钥对应位置的字母确定替换表
>
> 例如：  
> 明文：HELLO，密钥：KEY（长度 3），则分组为 “HEL”“LO”，对应密钥 “KEY”“KE”。  
> 每个字母按密钥字母在字母表中的偏移量加密（如 H + K 的偏移量 = H+10=R）。  
> 密钥：任意长度的短语或序列，密钥长度决定周期。
>
>
>
> 推荐一个密码破解网站
>
> [https://www.guballa.de/vigenere-solver](https://www.guballa.de/vigenere-solver)
>

#### ......

### md5
<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">MD5值是由32位由数字“0-9”和字母“a-f”所组成的字符串，字母大小写统一</font>

<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">16位值是取的是8~24位。</font>

<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);"></font>**<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">特征：</font>**

<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">有固定长度，一般是32位或者16位</font>

<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">由数字“0-9”和字母“a-f”组成</font>

**<font style="color:rgb(35, 38, 59);background-color:rgba(255, 255, 255, 0.9);">举例：</font>**

> 明文：flag  
> md5(32) = 327a6c4304ad5938eaf0efb6cc3e53dc  
> md5(16) = 04ad5938eaf0efb6
>

## 隐写类解题分析

### 通用思路
> ### 各类文件头：
> 题目可能将文件的文件头去掉这就需要我们补全文件头，也可以通过文件头尾确定文件类型，分离嵌入文件
>
>
>
> zip 文件头：50 4B 03 04 14 00 08 00  
> rar 文件头：52 61 72 21 (Rar!)               文件尾：C4 3D 7B 00 40 07 00  
> 7z  文件头：37 7A BC AF 27 1C  
>
> png 文件头：89504E47 0D0A1A0A    
>
> 文件尾：00000000 49454E44 AE426082  
> jpg 文件头：FF D8 FF E0  
>
> 文件尾：FF D9  
> gif 文件头：47 49 46 38 
>
> 文件尾：00 3B  
> bmp 文件头：42 4D
>
>
> mp3 文件头：49 44 33 03 00 00 00 00  
> wav 文件头：57 41 56 45   
>
> pyc 文件头：03 F3 0D 0A  
> xml 文件头：3C 3F 78 6D 6C  
> html 文件头：68 74 6D 6C 3E  
> pdf 文件头：255044462D312E
>

可以使用python库 magic识别文件类型

```python
import magic

# 安装  pip install python-magic-bin==0.4.14
# print(magic.from_buffer(open('guess', 'rb').read(2048), mime=True))  解决中文报错

m = magic.Magic()
file_path = "guess"
file_type = m.from_file(file_path)
print(file_type) 

# 输出 PNG image data, 835 x 706, 8-bit/color RGBA, non-interlaced

# 官方示例：
"""
magic is a wrapper around the libmagic file identification library.

See README for more information.

Usage:

>>> import magic
>>> magic.from_file("testdata/test.pdf")
'PDF document, version 1.2'
>>> magic.from_file("testdata/test.pdf", mime=True)
'application/pdf'
>>> magic.from_buffer(open("testdata/test.pdf").read(1024))
'PDF document, version 1.2'
>>>


"""
```

**grep用法：**

```shell
grep -E "关键词1|关键词2|关键词3" 文件名
搭配strings/cat
strings filename | grep -E "关键词1|关键词2|关键词3"
cat pass.txt | grep -E "pass|key"
输出：
:~/misc# cat pass.txt | grep -E "pass|key"
pass
key
pass
```

**exif:**

> **可能会将flag/password/key/init 放在exif里面常见在jpg里面，将jpg拖进010查看16进制数据有“Exif”则有exif数据**
>
> ****
>
> **查看exif:**
>
> ****
>
> **~/misc# exiftool mm.png **
>
> **apt install exiftool**
>
> ****
>
> ExifTool Version Number         : 12.40
>
> File Name                       : mm.png
>
> Directory                       : .
>
> File Size                       : 405 KiB
>
> File Modification Date/Time     : 2025:00:0 20:03:16+08:00
>
> File Access Date/Time           : 2025:00:0 20:21:00+08:00
>
> File Inode Change Date/Time     : 2025:00:0 20:03:16+08:00
>
> File Permissions                : -rw-r--r--
>
> File Type                       : PNG
>
> File Type Extension             : png
>
> MIME Type                       : image/png
>
> Image Width                     : 861
>
> Image Height                    : 436
>
> Bit Depth                       : 8
>
> Color Type                      : RGB with Alpha
>
> flag : flag{ssssss}
>
> Compression                     : Deflate/Inflate
>
> Filter                          : Adaptive
>
> Interlace                       : Noninterlaced
>
> SRGB Rendering                  : Perceptual
>
> Gamma                           : 2.2
>
> Pixels Per Unit X               : 5669
>
> Pixels Per Unit Y               : 5669
>
> Pixel Units                     : meters
>
> Warning                         : [minor] Trailer data after PNG IEND chunk
>
> Image Size                      : 861x436
>
> Megapixels                      : 0.375
>

以上是misc的一些常见信息收集，可以将这些工具和命令集成到shell，一键信息收集，后续做题我们还可以根据文件的不同添加其他的工具和命令

```shell
#!/bin/bash
# 作为misc的通用tool

# 配色
# 基本颜色
BRIGHT_BLUE_TEXT="\033[1;34m"

# 重置颜色
RESET="\033[0m"
# 蓝色
BLUE_LB() {
    echo "${BRIGHT_BLUE_TEXT}${1}${RESET}\n"
}

# exif数据提取
BLUE_LB "------------信息收集---------------"

BLUE_LB "exiftool"
exiftool "$1"

# 文件类型获取
BLUE_LB "文件类型"
file "$1"

# 关键字

CHARKEY="flag|FLAG|pass|pk|PK|Pk|ctf|CTF|KEY|key|txt|PASS"

# 关键字获取
BLUE_LB "关键字"
strings  "${1}" | grep "-E" "${CHARKEY}"
```

**输出：**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750131631266-6204e03c-48a8-4c97-845d-06d2758b8213.png)

经过这些基本上题目所给文件的类型，exif数据，关键字，有没有嵌入文件就都很清楚了，后面还会加入隐写检测，如stegpy,zsteg,OurSecret,steghide,outguess,以及png宽高检测等等，在misc分享的最后会将这个shell脚本完善，帮助我们快速的搜集文件的信息和获取隐写信息，解题快人一步，这个工具也能防遗忘，misc的隐写多种多样，这也是为什么编写shell脚本的原因

### 图片类隐写
资料收集：

一个隐写解析网站可以先放进去跑一下

[https://aperisolve.fr/](https://aperisolve.fr/)

stegpy：

> <font style="color:rgb(22, 18, 9);">安装：</font>
>
> <font style="color:rgb(22, 18, 9);">pip3 install stegpy</font>
>

> 使用：需要密码
>
> stegpy 1.png -p 
>

<font style="color:rgb(36, 41, 47);background-color:#FFFFFF;">Image Steganography：</font>

<font style="color:rgb(36, 41, 47);background-color:#FFFFFF;">使用Image Steganography decrypt</font>

npiet编程语言：

[https://www.bertnase.de/npiet/npiet-execute.php](https://www.bertnase.de/npiet/npiet-execute.php)

<font style="color:rgb(85, 85, 85);">将信息隐写在图片</font>

[https://stylesuxx.github.io/steganography/](https://stylesuxx.github.io/steganography/)

[https://www.a.tools/Tool.php?Id=100](https://www.a.tools/Tool.php?Id=100)

光栅图像：

[https://github.com/AabyssZG/Raster-Terminator](https://github.com/AabyssZG/Raster-Terminator)

工具站：[https://tools.jb51.net/aideddesign/img_add_info](https://tools.jb51.net/aideddesign/img_add_info)

DeEgger Embedder隐写 <font style="color:rgb(22, 18, 9);">DeEgger Embedder工具</font>

<font style="color:rgb(22, 18, 9);">把小说藏进图片 可以参考</font>[https://www.bilibili.com/video/BV1Ai4y1V7rg/?spm_id_from=333.999.0.0&vd_source=31399c09aa0c93655468bde7b13fcc03](https://www.bilibili.com/video/BV1Ai4y1V7rg/?spm_id_from=333.999.0.0&vd_source=31399c09aa0c93655468bde7b13fcc03)

Arnold猫脸变换：

原理：[https://www.jianshu.com/p/39727dbaffd9](https://www.jianshu.com/p/39727dbaffd9)

一个网上的脚本：

```python
from PIL import Image

def arnold(infile: str, outfile: str = None, a: int = 1, b: int = 1, shuffle_times: int = 1, reverse: bool = False) -> None:
    """
    Arnold猫脸变换函数

    Parameters:
        infile - 输入图像路径
        outfile - 输出图像路径
        a - Anrold 变换参数
        b - Anrold 变换参数
        shuffle_times - 置乱次数
        reverse - 逆变换
    """
    inimg = Image.open(infile)
    width, height = inimg.size
    indata = inimg.load()
    outimg = Image.new(inimg.mode, inimg.size)
    outdata = outimg.load()

    for _ in range(shuffle_times):
        for x in range(width):
            for y in range(height):
                if reverse:
                    nx = ((a * b + 1) * x - a * y) % width
                    ny = (y - b * x) % height
                else:
                    nx = (x + a * y) % width
                    ny = (b * x + (a * b + 1) * y) % height
                outdata[ny, nx] = indata[y, x]
    
    outimg.save(outfile if outfile else "arnold_"+infile, inimg.format)

arnold("before.png", "encode.png", 9, 39, 1)
arnold("encode.png", "decode.png", 9, 39, 1, True)

```

通常给a b数据可能给n 

二进制数据/rgb数据转图片:

图像逆序：

```python
infile = 'int.png'
outfile = 'out.png'

with open(infile, "rb") as fin:
    with open(outfile, "wb") as fout:
        fout.write(fin.read()[::-1])

```

#### png
**宽高：**

**题目会通过修改文件的宽高数据位来隐藏一些信息，我们可以通过比对crc位得到正确的宽高值**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750225698908-b103c10e-eb2e-4201-bddb-c2d936fc6fa4.png)

这是一个修改过宽高的图片的截图，我们可以看到仅仅有一句话其他什么也没有

而当我们正确的修改宽高后就可以看到隐藏在右下角的flag值

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750225802383-8794f857-21e4-40da-a9f3-96f54a4f7b33.png)

通常遇到比例奇怪的图片我们都可以尝试手动修改宽高

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750225899833-a5bdd2ac-e35a-4715-a381-dd0c74de1eaa.png)

1 处即为 宽度数据 2 处为高度数据 圈起来的地方为crc数据

当尝试发现可能被修改宽高后可以使用python脚本检测是否修改了宽高并修复得到正确宽高的图片

```python
import binascii
import itertools
import os
import struct
import zlib
import click


@click.command()
@click.option("-f","--file", required=True,help="file path")

def png_hw(file):
    # 修复png
    def modify_file_hex(file, position, new_hex_value):
                            try:
                                with open(file, 'rb') as f:
                                    content = f.read()
                                    hex_content = binascii.hexlify(content).decode()
                                    new_hex_content = hex_content[:position] + new_hex_value + hex_content[48:]
                                    modified_content = binascii.unhexlify(new_hex_content)
                                    output_file = os.path.join(os.path.dirname(file),
                                                                    'png_h_w_' + os.path.basename(file))
                                    with open(output_file, 'wb') as out_f:
                                        out_f.write(modified_content)
                                    return output_file
                            except FileNotFoundError:
                                return "文件不存在"
    try:
        png_data = open(f'{file}', 'rb').read()
        if png_data[:6].hex() != '89504e470d0a':
            print(f'非png文件')
        else:
            crc32key = zlib.crc32(png_data[12:29])  
            re_crc32 = int(png_data[29:33].hex(), 16) # 原始crc32值
            width = struct.unpack('>i', png_data[16:20])[0]
            height = struct.unpack('>i', png_data[20:24])[0]
            print(f'文件宽度：{width}, 文件高度：{height}')
            if crc32key == re_crc32:  
                print('文件宽高正确')
            else:
                print('文件宽高不正确，正在爆破宽高')
                for i, j in itertools.product(range(4095),
                                                range(
                                                    4095)):  
                    data = png_data[12:16] + struct.pack('>i', i) + struct.pack('>i', j) + png_data[24:29]
                    crc32 = zlib.crc32(data)
                    if crc32 == re_crc32:  
                        position = 32  
                        def pad_to_eight(s):
                            while len(s) < 8:
                                s = '0' + s
                            return s
                        w_out = pad_to_eight(hex(i)[2:])
                        h_out = pad_to_eight(hex(j)[2:])
                        new_hex_value = w_out + h_out
                        output_path = modify_file_hex(file, position, new_hex_value)
                        if output_path:
                            print(f'文件输出在{output_path}')
                        else:
                            print(f'文件错误')
    except ValueError:
        print("文件 error")
if __name__ == "__main__":
    png_hw()
```

**运行：**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750226142647-a19ff46a-da10-497b-b656-08860b14c8d4.png)

**文件分离：**

**binwalk**

这工具kali自带，可以在虚拟机安装一个kali

kali: [https://www.kali.org/get-kali/#kali-virtual-machines](https://www.kali.org/get-kali/#kali-virtual-machines)

vm虚拟机：[https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion](https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion)

vm下载需要注册，注册好无法登录去这里的mydownloads

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750226832605-2f428c4a-0442-42ae-8d20-98bda2d2eab9.png)

**用法：**

```shell
binwalk -e filename
```

**foremost:**

> sudo apt install foremost -y  # 安装foremost
>

**用法：**

```shell
foremost -i filename -o outpath
```

**盲水印：**

**单图盲水印：可以使用如下软件**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750227659203-a6b9f18a-7544-452e-9fd8-5d823664dd31.png)

[**https://www.123912.com/s/f2HzTd-9cz03**](https://www.123912.com/s/f2HzTd-9cz03)**提取码:FHgq**

**还有一个java盲水印工具 **[**https://github.com/ww23/BlindWatermark**](https://github.com/ww23/BlindWatermark)

**java -jar BlindWatermark-v0.0.3-windows-x86_64-gpu.jar decode -c gakki-dct-text-ec.jpg gakki-dct-text-dc.jpg**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750228630153-63c0463d-99e7-40a1-8677-19e0ba88161f.png)

**双图盲水印：**

**工具github地址：**

[**https://github.com/chishaxie/BlindWaterMark#blindwatermark**](https://github.com/chishaxie/BlindWaterMark#blindwatermark)

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750228030031-36c0e674-96af-4199-844e-0bd2291f6c4d.png)

另一个gui化的[https://github.com/fire-keeper/BlindWatermark](https://github.com/fire-keeper/BlindWatermark)

lsb隐写：

在png图片中，包含256的三次方个颜色，即16777216种，人类的眼睛可以区分约1,000万种不同的颜色，剩下无法区分的颜色就有6777216

LSB隐写就是修改RGB颜色分量的最低二进制位也就是最低有效位（LSB），而人类的眼睛不会注意到这前后的变化，我们仅对RGB中的最低位进行修改，如当前像素位点最后一位修改成1,1，0.则上述RGB变成218->219：

上述变化很难用肉眼察觉到，而且每一个像素位点携带了一位信息，那么我们可以利用八个字节的最低位存储一个比特信息，而该比特信息则可以转化为ASCII字符，从而达到隐写信息的目的

**zsteg:**

> 安装：
>
> github地址 [https://github.com/zed-0xff/zsteg](https://github.com/zed-0xff/zsteg)
>
> gem install zsteg
>

**主要用来检测png的lsb隐写，wbstego**

**StegSolve:**

**同样可以查看lsb，可以查看jpg...**

**在遇到题目给两张图片的时候亦可以使用他进行双图xor等**

**IDAT 块:**

**查看idat块是否正确，是否有多余的，可能为别的图像的数据块**

```shell
pngcheck file
```

#### jpg
**<font style="color:rgb(22, 18, 9);">OurSecret隐写：</font>**

**<font style="color:rgb(22, 18, 9);">特征明显，有如下数据</font>**

```shell
9E 97 BA 2A 00 80 88 C9 A3 70 97 5B A2 E4 99 B8
C1 78 72 0F 88 DD DC 34 2B 4E 7D 31 7F B5 E8 70
39 A8 B8 42 75 68 71 91

```

有密码，可以无密码

**stegdetect:**

stegdetect.exe -t jopi -s 10.0 1.jpg

检测加密

**silenteye：**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750231191904-f3d178e3-76b7-4707-acff-2a99905bf82a.png)

**steghide：**

```bash
steghide extract -sf filename -p passwd
```

**<font style="color:rgb(44, 63, 81);">JPHS：</font>**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750231214798-d09b16fc-f243-48c2-aa00-529fd548a942.png)

**<font style="color:rgb(85, 85, 85);">outguess：</font>**

```bash
outguess -k "pass" -r 1.jpg flag.txt
#-k 密钥
#flag.txt 保存位置
```

**<font style="color:rgb(85, 85, 85);">pixeljihad：</font>**

**<font style="color:rgb(85, 85, 85);">在线：</font>**[**https://sekao.net/pixeljihad/**](https://sekao.net/pixeljihad/)

**F5-steganography:**

```bash
#有密码
java Extract 1.jpg -p passwd
#无密码
java Extract 1.jpg
#数据会放到F5文件夹的output.txt

```

**JPG宽高隐写:**

**因为jpg和png不同，无法爆破crc确定正确的宽高只能手动修改**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750231409809-e60de58c-012e-46e8-becf-a4fd75b872ba.png)

#### bmp
**宽高：**

可以使用gimp修改

bmp文件头去掉

**<font style="color:rgb(36, 41, 47);background-color:#FFFFFF;">silenteye：同上面的jpg</font>**

**<font style="color:rgb(36, 41, 47);background-color:#FFFFFF;">wbStego4open: 同上</font>**

#### gif
**gif分离：**

```shell
convert flag.gif flag.png
```

**帧间隔：**

```bash
identify -format "%s %T \n" flag.gif 
```

#### ......

### 音视频隐写
[https://www.123912.com/s/f2HzTd-ZhL03](https://www.123912.com/s/f2HzTd-ZhL03)提取码:LCtD

#### wav
**<font style="color:rgb(36, 41, 47);">silenteye:</font>**

<font style="color:rgb(36, 41, 47);">可能是silenteye隐写,使用如同jpg，有密匙使用密匙解</font>

**<font style="color:rgb(36, 41, 47);">deepsound：</font>**

使用deepsound 打开，如果需要密码说明就是 deepsound 隐写，有密钥直接填入密钥解密即可

如果是 deepsound 隐写但没有密钥，这个时候就可有使用deepsound2john脚本获取wav文件的哈希值

然后用john爆破hash

用法: john 1.txt

> https://github.com/openwall/john/blob/bleeding-jumbo/run/deepsound2john.py
>

**sstv：**

工具：[https://github.com/colaclanth/sstv](https://github.com/colaclanth/sstv)

可以使用rx-sstv

也可以使用集成的工具

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1752725113336-51e85718-bce8-45c3-8c4e-38b9775ca8e3.png)

**<font style="color:rgb(22, 18, 9);">电话音分析(DTMF)：</font>**

<font style="color:rgb(22, 18, 9);">使用工具：dtmf2num.exe</font>

<font style="color:rgb(22, 18, 9);">用法：dtmf2num.exe xxx.wav</font>

**<font style="color:rgb(22, 18, 9);">Audacity：</font>**

<font style="color:rgb(22, 18, 9);">使用Audacity.exe打开查看是否有字符串等信息</font>

**<font style="color:rgb(22, 18, 9);">steghide：</font>**

<font style="color:rgb(22, 18, 9);">也可能是steghide</font>

<font style="color:rgb(22, 18, 9);">用法：</font>

```bash
steghide extract -sf filename -p passwd
```

#### mp3
**<font style="color:rgb(22, 18, 9);">mp3stego：</font>**

<font style="color:rgb(22, 18, 9);">工具地址：</font>[https://www.petitcolas.net/steganography/mp3stego/](https://www.petitcolas.net/steganography/mp3stego/)

用法：

> decode -X -P pass sound.mp3     
> -X 是提取出隐写的文件  
> pass是解密时需要的密码   
> sound.mp3是待处理的MP3文件  
> # mp3stego可以使用无密码进行隐写
>

**stegpy：**

```bash
stegpy 1.wav -p
```

**<font style="color:rgb(22, 18, 9);">DeEgger Embedder：</font>**

<font style="color:rgb(22, 18, 9);">地址：</font>[https://www.softpedia.com/get/Security/Encrypting/DeEgger-Embedder.shtml](https://www.softpedia.com/get/Security/Encrypting/DeEgger-Embedder.shtml)

### 文档类隐写

#### pdf
**嵌入文件：**

使用binwalk 或者 foremost

**<font style="color:rgb(36, 41, 47);">wbStego4open:</font>**

<font style="color:rgb(22, 18, 9);">使用</font><font style="color:rgb(36, 41, 47);">wbStego4open</font><font style="color:rgb(22, 18, 9);">带密钥</font>

**<font style="color:rgb(22, 18, 9);">有密码：</font>**

<font style="color:rgb(22, 18, 9);">使用pdfcrack爆破密码（Ubuntu: apt install pdfcrack）</font>

```bash
pdfcrack -f enc.pdf -w rockyou.txt
```

#### word
可能将文字隐藏，全选修改背景和字体颜色即可看到隐藏的

使用binwalk分离附加的文件

利用行距隐写将行距的不用转化为01解摩斯密码（如：<font style="color:rgb(22, 18, 9);">ISCC2023-汤姆历险记 </font>）

#### ppt
最常见的binwalk分离

#### excel
<font style="color:rgb(22, 18, 9);">使用记事本打开查找flag</font>

<font style="color:rgb(22, 18, 9);">查看单元格的不同，将不同的格分别转化为黑白格组成二维码</font>

<font style="color:rgb(22, 18, 9);">binwalk</font>

#### ......

### 文本类隐写

#### 零宽
零宽隐写是一种利用零宽度字符在文本中隐藏信息的技术，这些字符在视觉上不可见，但可以存储和传递隐秘信息。

可以使用在线网站：

[https://tool.bfw.wiki/tool/1695021695027599.html](https://tool.bfw.wiki/tool/1695021695027599.html)

[https://www.hanloth.cn/tool/zero-width-secret](https://www.hanloth.cn/tool/zero-width-secret)

或者集成工具：

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1752726462853-d166bc78-1150-4ae1-a05a-55c02deb39e8.png)

#### base隐写
**可以使用集成工具：**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1752726579560-89fc51c7-029d-43cd-acce-214b48528f67.png)

#### ......
**<font style="color:rgb(22, 18, 9);">snow隐写：</font>**

<font style="color:rgb(22, 18, 9);">SNOW.EXE -C -p password flag.txt </font>

**<font style="color:rgb(22, 18, 9);">垃圾邮件隐写(spammimic)：</font>**

<font style="color:rgb(22, 18, 9);">使用在线网站解密：</font>

[<font style="color:rgb(35, 118, 183);">https://www.spammimic.com/</font>](https://www.spammimic.com/)

**文字隐写：**

在线网站：

[https://toolshu.com/hide-text](https://toolshu.com/hide-text)

### ......

## 流量分析
使用Wireshark.exe打开直接搜索

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1752726760518-dc6ab77c-2709-4d3e-a171-cb3f24b4cee0.png)

或者导出文件

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1752726835375-1cb334d9-8019-40c9-886e-6faa7cb4fe46.png)

## 取证题分析
使用vol解析

## 压缩包题分析

### 伪加密

```python
ZIP伪加密是一种通过修改ZIP文件头部的加密标志位，使文件被识别为加密压缩包的技术。实际上，这种加密并不真正保护文件内容，因此被称为“伪加密”。以下是ZIP伪加密的原理及其处理方法。

ZIP文件结构与伪加密原理

一个ZIP文件通常由三个部分组成：

压缩源文件数据区：包含文件的实际数据。

压缩源文件目录区：记录文件的元信息。

压缩源文件目录结束标志：标记目录的结束。

在ZIP文件中，加密属性由“全局方式位标记”决定：

无加密：全局方式位标记为00 00。

伪加密：数据区的全局方式位标记为00 00，但目录区的标记被修改为09 00。

真加密：数据区和目录区的全局方式位标记均为09 00。

伪加密的核心在于修改目录区的标记，使其显示为加密状态，但实际数据并未加密。
```

直接使用集成工具

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1752727513475-9c47a687-f1b9-45fc-bd50-161b3b61c249.png)

### 爆破
**archpr:**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1752727604255-934f859f-f00d-4df1-95d5-bbc13f0cf198.png)

### 明文爆破
也可使用上述工具

要求：

<font style="color:rgb(51, 51, 51);">至少已知明文的12个字节及偏移，其中至少8字节需要连续。</font>

<font style="color:rgb(51, 51, 51);">明文对应的文件加密方式为ZipCrypto Store</font>

**<font style="color:rgb(51, 51, 51);">bkcrack:</font>**

[https://github.com/kimci86/bkcrack](https://github.com/kimci86/bkcrack)

### crc爆破
<font style="color:rgb(22, 18, 9);">压缩包中文件比较小只有几字节</font>

<font style="color:rgb(22, 18, 9);">工具：</font>

[https://github.com/AabyssZG/CRC32-Tools](https://github.com/AabyssZG/CRC32-Tools)

[https://github.com/theonlypwner/crc32](https://github.com/theonlypwner/crc32)

### ......

# CRYPTO

## RSA

### RSA基础理论及加解密过程
工具集成了一些常见的rsa攻击方式 只需要了解相关攻击即可使用

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1753933177946-d2a90513-cc04-4aa2-be1f-53606026646e.png)

<font style="color:rgb(32, 33, 34);">对极大整数做</font>[<font style="color:rgb(51, 102, 204);">因数分解</font>](https://zh.wikipedia.org/wiki/%E5%9B%A0%E6%95%B0%E5%88%86%E8%A7%A3)<font style="color:rgb(32, 33, 34);">的难度决定了 RSA 算法的可靠性。换言之，对一极大整数做因数分解愈困难，RSA 算法愈可靠。假如有人找到一种快速因数分解的算法的话，那么用 RSA 加密的信息的可靠性就会极度下降。但找到这样的算法的可能性是非常小的。今天只有短的 RSA 钥匙才可能被强力方式破解。到2020年为止，世界上还没有任何可靠的攻击RSA算法的方式。只要其钥匙的长度足够长，用RSA加密的信息实际上是不能被破解的。</font>

维基百科：

[https://zh.wikipedia.org/wiki/RSA%E5%8A%A0%E5%AF%86%E6%BC%94%E7%AE%97%E6%B3%95](https://zh.wikipedia.org/wiki/RSA%E5%8A%A0%E5%AF%86%E6%BC%94%E7%AE%97%E6%B3%95)

python的简单实现：

```python
from Crypto.Util.number import getPrime, inverse, bytes_to_long, long_to_bytes

flag =  b'flag{RSA}'

# 生成1024位的素数p和q

p = getPrime(1024)
q = getPrime(1024)

# 计算n, e, phi, d和c
n = p * q

e = 65537

phi = (p - 1) * (q - 1)

assert GCD(e, phi) == 1, "该e不满足互素条件"

d = inverse(e, phi)

c = pow(bytes_to_long(flag), e, n)

m = pow(c, d, n)

print(f'n = {n}')
print(f'e = {e}')   
print(f'd = {d}')
print(f'c = {c}')
print(f'm = {long_to_bytes(m)}')
```

rsa题目常见的参数 

p 素数生成n

q 素数生成n

pq 是解题的关键 通常要求的参数

n 与e组成公钥

e 与n组成公钥

c 加密后的密文

phi n的欧拉 =(p-1)*(q-1) pq = n p+q pq -p -q +1 = pq - (p+q) + 1 

d  私钥 解题的关键

m 明文

通常题目会给 n e c 

我们可以根据这三个参数来判断使用那些攻击方式

一开始我们可以尝试分解N，如果n不大

[http://www.factordb.com/](http://www.factordb.com/)

这是一个记录了很多已经被分解的n的pq

我们也可以使用yafu分解，如果pq相差较大或小的时候，可以根据题目所给加密代码判断

[https://sourceforge.net/projects/yafu/](https://sourceforge.net/projects/yafu/)

我们还需要学习一些python库

Crypto

gmpy2

### 常见攻击方式

#### <font style="color:rgb(0, 0, 0);">小明文攻击</font>
当题目中N特别大的时候可以尝试

我们已知 Ⅰ:  C  <font style="color:rgb(0, 0, 0);">≡</font>![image](https://cdn.nlark.com/yuque/__latex/cc221ed71b2d6a5f6487c0d93be71c3d.svg)<font style="color:rgb(0, 0, 0);">(mod N)</font>

<font style="color:rgb(0, 0, 0);">当m很小的时候 m的e次方小于n</font>

<font style="color:rgb(0, 0, 0);">所以 c 就等于 m的e次方 此时我们只要将 c 开 e 次方就可以得到 m</font>

<font style="color:rgb(0, 0, 0);">这里使用 gmpy2 库的iroot开方</font>

```python
from Crypto.Util.number import *
from gmpy2 import *
n  = 536410484994483033093334003836655729325470269375524009439921349251765426879326472420715343135213685847853149465047363004844978980705334818310367627899054282724091430760574321302693735313741776534635308880108579425210969875273787315835179223662471838419622222586196334875552681127482220681804218077447446727632367288719418398225173584249649494060944903031644643599350735559974998992685357629587918116319437983541031003274274249512385723959144711034887286740398048911255492577006594659820438597055144909808217806214389981467817007584648955570726162669186034727073111376869516381199706615431972535815322666741187757365776611420640881256943303112723909875163327558585208160248953717008905206187852681531673607531360656420914879152163720617911529983435735678874123738624814506966909449518581239944997840945458848686624613184987748822188025864390108649415309566456540845277892075600527410134107469406816659137099034223840641145291291677316961839250222786771084598108203101897949775024306470936804403534408830935782941709356062377127100322538567707179546810871854386057481906331948667458888491116697493079241029509563403449393692443545157249665866189068291745976311888965264882340009888119575540460672793226773934767675512684750592502994661
e = 47
c = 229899396883582392364871905906445296949203163435377967308523386636507105732351552139686055293875453912112843930875659740397422297275613832964886182478284228932337946906215427434632071627272673570051303664678550765869183098488754645162034875760803916176659931431903280877040008151839312486086810338837714295821068677830038145047288362507454852643283361570635475479731085221630599511037989875119938896391192076787426053096532792131784563523065082875308622036981017576697767085294161885999051064464805324234829382111945083257918268260979566515252826957333562648074716098524243209378279602403795364197351006272703919005850152191380237640254523031072133802051271379417062521178212883200712566363108988562038188056490055724405896019781505695009412712690784013380990981185039802898643638127923786296260202685639474550000877637714438089700174399902960859666510114240835250541384360368049671274643421485904308653603924744567918821295775350084960806905039253932125210810019431964659889918601526879604439206186643987785399968027152305034576184766368079201408412844596024313611950909884330051927770353597750655703028328638756559133666564620074677469304330050449745861462898383722361080035329755112868572844306365995005218909407333254086037  

m = iroot(c, e)

print(long_to_bytes(m[0]))
```

#### <font style="color:rgb(0, 0, 0);">低加密指数攻击</font>
由 Ⅰ 消去模 得到 ![image](https://cdn.nlark.com/yuque/__latex/5408886ac0518174dec52ede9a1a5951.svg)= c + k*n

当e很小的时候 我们可以爆破k 得到正确的 ![image](https://cdn.nlark.com/yuque/__latex/5408886ac0518174dec52ede9a1a5951.svg)

```python
from Crypto.Util.number import *
from gmpy2 import *
n = 25066689877776679233022203369122860358311144108034322786249336304184718167290635002070039262490792542129164733263246201499413220464411226682235152645481523633440451076347588502189820875766207732385081347542902014379448935897761402426197951109899225264278881605284920398145164965059125758041113782043
e = 5
c = 9580937997026657207695606535792321409809664111257153374644767194117132680120146044970386750643915697649050660680091489013318267184823888266207920970701381149337870449324937658700572686851552653818796958133992739190614740958850104564209920508542730206551286453342339610980738869413911612550009452577
for k in range(100000):
    me = c + k*n
    res = iroot(me, e) # iroot返回 一个元组，第一个元素是整数的整数根，第二个元素是布尔值，表示是否是整数根
    if res[1]:
        m = res[0]
        break
print(long_to_bytes(m))
```

#### <font style="color:rgb(0, 0, 0);">Rabin算法攻击</font>
一个显著的特征 e为2

```python
from Crypto.Util.number import *
from gmpy2 import *

p = 
q = 
e = 2
c = 

def rabin_attack(c, n, p, q):
    c1 = powmod(c, (p+1)//4, p)
    c2 = powmod(c, (q+1)//4, q)
    cp1 = p - c1
    cp2 = q - c2

    t1 = invert(p, q)
    t2 = invert(q, p)

    m1 = (q*c1*c2 + p*c2*t1) % n
    m2 = (q*c1*t2 + p*cp2*t1) % n
    m3 = (q*cp1*t2 + p*c2*t1) % n
    m4 = (q*cp1*t2 + p*cp2*t1) % n

    return m1, m2, m3, m4

ms = rabin_attack(c, p*q, p, q)

for m in ms:
    print(long_to_bytes(m))
```

#### <font style="color:rgb(0, 0, 0);">Wiener攻击</font>
[https://github.com/pablocelayes/rsa-wiener-attack](https://github.com/pablocelayes/rsa-wiener-attack)

```python
from Crypto.Util.number import *
from gmpy2 import *

n = 
e = 
c = 

class ContinuedFraction():
    def __init__(self, numerator, denumerator):
        self.numberlist = []  
        self.fractionlist = []  
        self.GenerateNumberList(numerator, denumerator)
        self.GenerateFractionList()

    def GenerateNumberList(self, numerator, denumerator):
        while numerator != 1:
            quotient = numerator // denumerator
            remainder = numerator % denumerator
            self.numberlist.append(quotient)
            numerator = denumerator
            denumerator = remainder

    def GenerateFractionList(self):
        self.fractionlist.append([self.numberlist[0], 1])
        for i in range(1, len(self.numberlist)):
            numerator = self.numberlist[i]
            denumerator = 1
            for j in range(i):
                temp = numerator
                numerator = denumerator + numerator * self.numberlist[i - j - 1]
                denumerator = temp
            self.fractionlist.append([numerator, denumerator])


a = ContinuedFraction(e, n)
for k, d in a.fractionlist:
    m = powmod(c, d, n)
    flag = long_to_bytes(m)
    
    if b'flag' in flag:  #根据具体的flag头更改
        print(flag)
```

#### <font style="color:rgb(0, 0, 0);">低加密指数广播攻击</font>
<font style="color:rgb(51, 51, 51);">当有多组n，c的时候，且e小</font>

```python
import libnum
from gmpy2 import invert, gcd, iroot

def op(x):
    res = 1
    for i in x:
        res *= i
    return res

def CRT(m, a):
    assert (len(m) == len(a))
    M = op(m)
    sum = 0
    for m, a in zip(m, a):
        Mi = M // m
        ti = invert(Mi, m)
        sum += a * ti * Mi
    return sum % M
def GCRT(m, a):
    assert (len(m) == len(a))
    curm, cura = m[0], a[0]
    for m, a in zip(m[1:], a[1:]):
        d = gcd(curm, m)
        c = a - cura
        assert (c % d == 0)
        K = c // d * invert(curm // d, m // d)
        cura += curm * K
        curm = curm * m // d
    return cura % curm

e= 23
n= [, , , , , , ]
c= [, , , , , , ]

m = CRT(n, c)
m1 = iroot(m, e)  # 开e次方
print(m1)
print(libnum.n2s(int(m1[0])))
```

#### <font style="color:rgb(0, 0, 0);">p-1光滑攻击</font>
<font style="color:rgb(51, 51, 51);">光滑数：指可以分解为小素数乘积的正整数</font>

```python
from Crypto.Util.number import *
from gmpy2 import *
n =
e = 65537
c = 
a = 2
m = 2
while True:
    a = powmod(a, m, n)
    p = gcd(a-1, n)
    if p != 1 and p != n:
        break
    m += 1
print(p)
q = n // p

phi = (p-1)*(q-1)
d = invert(e, phi)
m = powmod(c, d, n)
print(long_to_bytes(m))
```

#### <font style="color:rgb(0, 0, 0);">p+1光滑攻击</font>

```python
from Crypto.Util.number import *
from gmpy2 import *
from itertools import count

n = 
e = 65537
c = 

def mlucas(v, a, n):
    v1, v2 = v, (v ** 2 - 2) % n
    for bit in bin(a)[3:]: v1, v2 = ((v1 ** 2 - 2) % n, (v1 * v2 - v) % n) if bit == "0" else (
        (v1 * v2 - v) % n, (v2 ** 2 - 2) % n)
    return v1

def primegen():
    yield 2
    yield 3
    yield 5
    yield 7
    yield 11
    yield 13
    ps = primegen()  # yay recursion
    p = ps.__next__() and ps.__next__()
    q, sieve, n = p ** 2, {}, 13
    while True:
        if n not in sieve:
            if n < q:
                yield n
            else:
                next, step = q + 2 * p, 2 * p
                while next in sieve:
                    next += step
                sieve[next] = step
                p = ps.__next__()
                q = p ** 2
        else:
            step = sieve.pop(n)
            next = n + step
            while next in sieve:
                next += step
            sieve[next] = step
        n += 2

def ilog(x, b):  # greatest integer l such that b**l <= x.
    l = 0
    while x >= b:
        x /= b
        l += 1
    return l

def attack(n):
    for v in count(1):
        for p in primegen():
            e = ilog(isqrt(n), p)
            if e == 0:
                break
            for _ in range(e):
                v = mlucas(v, p, n)
            g = gcd(v - 2, n)
            if 1 < g < n:
                return int(g), int(n // g)  # g|n
            if g == n:
                break

p, q = attack(n)


phi = (p-1)*(q-1)
d = invert(e, phi)
m = powmod(c, d, n)
print(long_to_bytes(m))
```

#### <font style="color:rgb(0, 0, 0);">共模攻击</font>
题目给出两对e c 公用同一个n

```python
from gmpy2 import *
from Crypto.Util.number import *

n = 

e1 = 
e2 = 

c1 = 
c2 = 

_, s1, s2 = gcdext(e1, e2)

m = powmod(c1, s1, n) * powmod(c2, s2, n) % n
print(long_to_bytes(m))
```

#### <font style="color:rgb(0, 0, 0);">dp&dq泄露攻击</font>

```python
import gmpy2
import libnum
def decrypt(dp,dq,p,q,c):
    InvQ = gmpy2.invert(q, p)
    mp = pow(c, dp, p)
    mq = pow(c, dq, q)
    m = (((mp-mq)*InvQ) % p)*q+mq
    print(libnum.n2s(int(m)).decode())
p= 
q= 
dq= 
dp= 
c= 
decrypt(dp,dq,p,q,c) 
```

#### <font style="color:rgb(0, 0, 0);">dp泄露攻击</font>

```python
import libnum
import gmpy2
n= 
e= 65537
dp= 
c= 
for i in range(1,65535):
    p=(dp*e-1)//i+1
    if n%p==0:
        q=n//p
        break
phi_n= (p-1)*(q-1)
d=gmpy2.invert(e,phi_n)
m=pow(c,d,n)
print(m)
flag=libnum.n2s(int(m)).decode()
print(flag)
```

#### <font style="color:rgb(0, 0, 0);">e很大的dp泄露攻击</font>

```python
from Crypto.Util.number import *
from gmpy2 import *

n = 
e = 
c = 
dp = 

m = #随机
p = gcd(powmod(m, e*dp, n) - m, n)
q = n // p
d = invert(e, (p - 1) * (q - 1))
m = powmod(c, d, n)
print(long_to_bytes(m))
```

#### <font style="color:rgb(0, 0, 0);">已知明文高位攻击</font>
需要sage

[https://mirrors.aliyun.com/sagemath/win/index.html](https://mirrors.aliyun.com/sagemath/win/index.html)

m高位已知

```python
import libnum
def phase2(high_m, n, c):
    R.<x> = PolynomialRing(Zmod(n), implementation='NTL')
    m = high_m + x
    M = m((m^3 - c).small_roots()[0])
    print(libnum.n2s(int(M)))
n= 
e= 3
c= 
high_m= 

phase2(high_m, n, c) 
```

#### <font style="color:rgb(0, 0, 0);">已知p高位攻击</font>
需要sage

```python
n = 
p4=
e = 0x10001
pbits = 1024
kbits = pbits - p4.nbits()
print(p4.nbits())
p4 = p4 << kbits
PR.<x> = PolynomialRing(Zmod(n))
f = x + p4
roots = f.small_roots(X=2^kbits, beta=0.4)
if roots:
    p = p4+int(roots[0])
    print (n)
    print (p)
    print (n/p)
```

#### <font style="color:rgb(0, 0, 0);">AMM算法</font>
好文章[https://xz.aliyun.com/news/13908](https://xz.aliyun.com/news/13908)

```python

from Crypto.Util.number import *
from gmpy2 import *
import random
import math

n = 
c = 
p =    
q = 
e = 

def onemod(e, q):
    p = random.randint(1, q-1)
    while(powmod(p, (q-1)//e, q) == 1):  # (r,s)=1
        p = random.randint(1, q)
    return p

def AMM_rth(o, r, q):  # r|(q-1
    assert((q-1) % r == 0)
    p = onemod(r, q)

    t = 0
    s = q-1
    while(s % r == 0):
        s = s//r
        t += 1
    k = 1
    while((s*k+1) % r != 0):
        k += 1
    alp = (s*k+1)//r

    a = powmod(p, r**(t-1)*s, q)
    b = powmod(o, r*a-1, q)
    c = powmod(p, s, q)
    h = 1

    for i in range(1, t-1):
        d = powmod(int(b), r**(t-1-i), q)
        if d == 1:
            j = 0
        else:
            j = (-math.log(d, a)) % r
        b = (b*(c**(r*j))) % q
        h = (h*c**j) % q
        c = (c*r) % q
    result = (powmod(o, alp, q)*h)
    return result

def ALL_Solution(m, q, rt, cq, e):
    mp = []
    for pr in rt:
        r = (pr*m) % q
        # assert(pow(r, e, q) == cq)
        mp.append(r)
    return mp


def calc(mp, mq, e, p, q):
    i = 1
    j = 1
    t1 = invert(q, p)
    t2 = invert(p, q)
    for mp1 in mp:
        for mq1 in mq:
            j += 1
            if j % 100000 == 0:
                print(j)
            ans = (mp1*t1*q+mq1*t2*p) % (p*q)
            if check(ans):
                return
    return


def check(m):
    try:
        a = long_to_bytes(m)
        if b'NSSCTF' in a:
            print(a)
            return True
        else:
            return False
    except:
        return False


def ALL_ROOT2(r, q):  # use function set() and .add() ensure that the generated elements are not repeated
    li = set()
    while(len(li) < r):
        p = powmod(random.randint(1, q-1), (q-1)//r, q)
        li.add(p)
    return li

cp = c % p
cq = c % q

mp = AMM_rth(cp, e, p)  # AMM算法得到一个解
mq = AMM_rth(cq, e, q)

rt1 = ALL_ROOT2(e, p)  # 得到所有的ri，即(ri*mp)^e%p = 1
rt2 = ALL_ROOT2(e, q)

amp = ALL_Solution(mp, p, rt1, cp, e)  # 得到所有的mp
amq = ALL_Solution(mq, q, rt2, cq, e)

calc(amp, amq, e, p, q)  # 俩俩CRT
```

#### <font style="color:rgb(51, 51, 51);">剪枝</font>
<font style="color:rgb(51, 51, 51);">a1^b1：</font>

```python
from Crypto.Util.number import *
import sys

sys.setrecursionlimit(1500)

# part1,剪枝
a1 = 
b1 = 
c1 = 
e = 65537
a1 = "0" + str(bin(a1)[2:])


def find(p, q):
    l = len(p)
    tmp0 = p + (1024 - l) * "0"
    tmp1 = p + (1024 - l) * "1"
    tmq0 = q + (1024 - l) * "0"
    tmq1 = q + (1024 - l) * "1"
    if (int(tmp0, 2) < int(tmq0, 2)):
        return
    if (int(tmp0, 2) * int(tmq0, 2) > b1):
        return
    elif (int(tmp1, 2) * int(tmq1, 2) < b1):
        return

    if (l == 1024):
        pp = int(tmp0, 2)
        qq = int(tmq0, 2)
        d = inverse(e, (pp - 1) * (qq - 1))
        m = long_to_bytes(pow(c1, d, pp * qq))
        print(str(m)[2:-1], end="")

    else:
        if (a1[l] == "1"):
            find(p + "1", q + "0")
            find(p + "0", q + "1")
        else:
            find(p + "0", q + "0")
            find(p + "1", q + "1")


tempp = ""
tempq = ""
find(tempp, tempq)
```

<font style="color:rgb(51, 51, 51);">p ^ _q：</font>

<font style="color:rgb(51, 51, 51);">p与q的反方向二进制的异或值</font>

```python
from Crypto.Util.number import *
import sys
sys.setrecursionlimit(1500)

pxorq = 
n =
c = 
e = 65537
pxorq = str(bin(pxorq)[2:]).zfill(256)
 
def find(ph,qh,pl,ql):
    l = len(ph)
    tmp0 = ph + (256-2*l)*"0" + pl
    tmp1 = ph + (256-2*l)*"1" + pl
    tmq0 = qh + (256-2*l)*"0" + ql
    tmq1 = qh + (256-2*l)*"1" + ql
    if(int(tmp0,2)*int(tmq0,2) > n):
        return 
    if(int(tmp1,2)*int(tmq1,2) < n):
        return
    if(int(pl,2)*int(ql,2) % (2**(l-1)) != n % (2**(l-1))):
        return

    if(l == 128):
        pp0 = int(tmp0,2)
        if(n % pp0 == 0):
            pf = pp0
            qf = n//pp0
            phi = (pf-1)*(qf-1)
            d = inverse(e,phi)
            m1 = pow(c,d,n)
            print(long_to_bytes(m1))
            exit()

    else:
        if(pxorq[l] == "1" and pxorq[255-l] == "1"):
            find(ph+"1",qh+"0","1"+pl,"0"+ql)
            find(ph+"0",qh+"0","1"+pl,"1"+ql)
            find(ph+"1",qh+"1","0"+pl,"0"+ql)
            find(ph+"0",qh+"1","0"+pl,"1"+ql)
        elif(pxorq[l] == "1" and pxorq[255-l] == "0"):
            find(ph+"1",qh+"0","0"+pl,"0"+ql)
            find(ph+"0",qh+"0","0"+pl,"1"+ql)
            find(ph+"1",qh+"1","1"+pl,"0"+ql)
            find(ph+"0",qh+"1","1"+pl,"1"+ql)
        elif(pxorq[l] == "0" and pxorq[255-l] == "1"):
            find(ph+"0",qh+"0","1"+pl,"0"+ql)
            find(ph+"0",qh+"1","0"+pl,"0"+ql)
            find(ph+"1",qh+"0","1"+pl,"1"+ql)
            find(ph+"1",qh+"1","0"+pl,"1"+ql)
        elif(pxorq[l] == "0" and pxorq[255-l] == "0"):
            find(ph+"0",qh+"0","0"+pl,"0"+ql)
            find(ph+"1",qh+"0","0"+pl,"1"+ql)
            find(ph+"0",qh+"1","1"+pl,"0"+ql)
            find(ph+"1",qh+"1","1"+pl,"1"+ql)

find("1","1","1","1")
```

## <font style="color:rgb(79, 79, 79);">DSA</font>

### 原理及加解密过程
[https://zh.wikipedia.org/wiki/%E6%95%B0%E5%AD%97%E7%AD%BE%E5%90%8D%E7%AE%97%E6%B3%95](https://zh.wikipedia.org/wiki/%E6%95%B0%E5%AD%97%E7%AD%BE%E5%90%8D%E7%AE%97%E6%B3%95)

## <font style="color:rgb(79, 79, 79);">ECC</font>

### 原理及加解密过程

## <font style="color:rgb(79, 79, 79);">AES/DES</font>

## ......

## 脚本:

```python
#!/bin/bash
# 作为misc的通用tools
# huihuilikaile 20250425



# 设置颜色信息
# 基本文字颜色
BLACK_TEXT="\033[30m"
RED_TEXT="\033[31m"
GREEN_TEXT="\033[32m"
YELLOW_TEXT="\033[33m"
BLUE_TEXT="\033[34m"
PURPLE_TEXT="\033[35m"
CYAN_TEXT="\033[36m"
WHITE_TEXT="\033[37m"

# 基本背景颜色
BLACK_BG="\033[40m"
RED_BG="\033[41m"
GREEN_BG="\033[42m"
YELLOW_BG="\033[43m"
BLUE_BG="\033[44m"
PURPLE_BG="\033[45m"
CYAN_BG="\033[46m"
WHITE_BG="\033[47m"

# 亮色文字颜色
BRIGHT_BLACK_TEXT="\033[1;30m"
BRIGHT_RED_TEXT="\033[1;31m"
BRIGHT_GREEN_TEXT="\033[1;32m"
BRIGHT_YELLOW_TEXT="\033[1;33m"
BRIGHT_BLUE_TEXT="\033[1;34m"
BRIGHT_PURPLE_TEXT="\033[1;35m"
BRIGHT_CYAN_TEXT="\033[1;36m"
BRIGHT_WHITE_TEXT="\033[1;37m"

# 自定义 RGB 颜色
CUSTOM_RED_TEXT="\033[38;2;255;0;0m"
CUSTOM_GREEN_BG="\033[48;2;0;255;0m"

# 组合背景颜色

GREEN_WHITE_TEXT="\033[1;47;32m"
BLUE_WHITE_TEXT="\033[1;34;47m"
BLUE_GREE_TEXT="\033[34;42m"
# 重置颜色
RESET="\033[0m"

# 设置颜色函数

RED_B() {
    echo "${RED_TEXT}${1}${RESET}\n"
}

BLUE_B() {
    echo "${BLUE_TEXT}${1}${RESET}\n"
}

RED_LB() {
    echo "${BRIGHT_RED_TEXT}${1}${RESET}\n"
}

BLUE_LB() {
    echo "${BRIGHT_BLUE_TEXT}${1}${RESET}\n"
}

ALL_B() {
    echo "${BLUE_WHITE_TEXT}${1}${RESET}\n"
}

BLUE_GREE_B() {
    echo "${BLUE_GREE_TEXT}${1}${RESET}\n"
}

FENGE() {
    echo "${GREEN_TEXT}${1}${RESET}\n"
}

# 设置帮助信息
usage() {
    echo "Usage: $0 [-f <arg>] [-p <arg>] [-j <arg>] [-g <arg>] [-h]"
    echo "  -f filename  提供文件的类型,EXIF,关键字检测,文件隐藏(binwalk foremost)等信息"
    echo "  -p True/T/t  进行png相关的检测 "
    echo "  -j key  进行jpg相关的检测 "
    echo "  -g True/T/t  进行gif相关的检测 "
    echo "  -h 获取帮助"
    exit 1
}


# ANSI 转义码定义
RED='\033[0;31m'
GREEN='\033[0;32m'
YELLOW='\033[0;33m'
BLUE='\033[0;34m'
NC='\033[0m' # 重置颜色

# 函数：将文本添加带颜色的边框
add_colored_border() {
  local text="$1"
  local length=${#text}
  
  # 计算边框宽度（增加一些额外的空间）
  local border_width=$((length + 4))
  
  # 打印上边框
  printf "${BLUE_TEXT}+%0.s-" $(seq 1 $border_width)
  echo "--${NC}"
  
  # 打印文本行
  printf "${colBLUE_TEXTor} %s ${NC}\n" "$text"
  
  # 打印下边框
  printf "${BLUE_TEXT}+%0.s-" $(seq 1 $border_width)
  echo "--${NC}"
}

# 关键字

CHARKEY="flag|FLAG|pass|pk|PK|Pk|ctf|CTF|KEY|key|txt|PASS"

# 目录设置

binwalkout="binwalkoutfile"

foremostout="foremostoutfile"

# 字符匹配函数
grep_file() {
    outkeys=$(strings "${1}" | grep "-E" "${CHARKEY}")
    add_colored_border $outkeys
}
# 文件类型匹配
file_type() {
    file $1
}

# exif数据
exif_file() {
    exiftool "$1"
}



forf() {
    timefile=$(date +"%H%M%S")
    filename="${foremostout}/${timefile}_${1%%.*}"
    if [ -d $filename ]; then
        RED_LB "${RED_TEXT}目录${filename}不为空,重新创建:${RESET}"
        timefile=$(date +"%H%M%S")
        filename="${foremostout}/${timefile}_${1%%.*}"
        mkdir $filename
        BLUE_LB "新目录:${filename}"
        foremost "-i" "$1" "-o" "${filename}"
        FENGE "目录树: "
        tree $filename
    else
        mkdir $filename
        
        foremost "-i" "$1" "-o" "${filename}"

        BLUE_LB "\nforemost输出目录: ${filename}"

        FENGE "目录树: "
        tree $filename
    fi
}
#------------------图片相关---------------------
# OurSecret隐写检测
OurSecret_file() {
    # 模拟 xxd 输出
    xxd_output=$(xxd "-p" $1)

    # 待比对的十六进制数据
    target_hex="9e97ba2a008088c9a370975ba2e499b8c178720f88dddc342b4e7d317fb5e87039a8b84275687191"

    # 进行比对
    if echo "$xxd_output" | grep -q "$target_hex"; then
        RED_B "可能存在OurSecret"
    else
        BLUE_LB "不存在OurSecret隐写"
    fi
}


# 设置参数选项
while getopts ":f:p:j:g:b:h" opt; do
    case $opt in
        f)
            # BINWALK FOREMOST STRINGS GREP
            FENGE "-----------------信息收集-------------------"
            BLUE_GREE_B "文件类型检测:"
            file_type $OPTARG
            BLUE_GREE_B "关键字:"
            grep_file $OPTARG
            BLUE_GREE_B "exif数据:"
            exif_file $OPTARG
            BLUE_GREE_B "FOREMOST 分离结果:"
            forf $OPTARG
            f_name="$OPTARG"
            
            ;;
        p)
            PTRUE=true
            FENGE "-----------------PNG相关检测-------------------"
            BLUE_GREE_B "png宽高检测:"
            pnghwout=$(python3 "pnghw.py" "-f" "${f_name}")
            BLUE_LB $pnghwout
            BLUE_GREE_B "png IDAT快检测:"
            pngcheck "-v" "${f_name}"
            
            BLUE_GREE_B "OurSecret隐写检测:"
            OurSecret_file $f_name
            ;;
        j)
            BLUE_GREE_B "OurSecret隐写检测:"
            OurSecret_file $f_name
            BLUE_GREE_B "steghide未知密码隐写检测:"
            steghide "extract" "-sf" $f_name
            BLUE_GREE_B "outguess隐写检测:"
            outguess "-k" "$OPTARG" "-r"  $f_name "${f_name%%.*}.txt"
            BLUE_LB "输出文件为：${f_name%%.*}.txt"
            ;;
        g)
            BLUE_B "Option c$OPTARG"
            ;;
        g)
            BLUE_B "Option c$OPTARG"
            ;;
	    h)
	        usage
	        ;;
        \?)
            RED_LB "未知选项: -$OPTARG" >&2
            ;;
        :)
            RED_LB "提供给 -$OPTARG 选项一个参数." >&2
            ;;
    esac
done 
FENGE "-----------------储存资料-------------------"
cat "www.txt"
if [ "$PTRUE" = true ]; then
    BLUE_GREE_B "执行zsteg: "
    zsteg "-a" "$f_name"
fi

```

1, 47);background-color:#FFFFFF;">使用Image Steganography decrypt</font>

npiet编程语言：

[https://www.bertnase.de/npiet/npiet-execute.php](https://www.bertnase.de/npiet/npiet-execute.php)

<font style="color:rgb(85, 85, 85);">将信息隐写在图片</font>

[https://stylesuxx.github.io/steganography/](https://stylesuxx.github.io/steganography/)

[https://www.a.tools/Tool.php?Id=100](https://www.a.tools/Tool.php?Id=100)

光栅图像：

[https://github.com/AabyssZG/Raster-Terminator](https://github.com/AabyssZG/Raster-Terminator)

工具站：[https://tools.jb51.net/aideddesign/img_add_info](https://tools.jb51.net/aideddesign/img_add_info)

DeEgger Embedder隐写 <font style="color:rgb(22, 18, 9);">DeEgger Embedder工具</font>

<font style="color:rgb(22, 18, 9);">把小说藏进图片 可以参考</font>[https://www.bilibili.com/video/BV1Ai4y1V7rg/?spm_id_from=333.999.0.0&vd_source=31399c09aa0c93655468bde7b13fcc03](https://www.bilibili.com/video/BV1Ai4y1V7rg/?spm_id_from=333.999.0.0&vd_source=31399c09aa0c93655468bde7b13fcc03)

Arnold猫脸变换：

原理：[https://www.jianshu.com/p/39727dbaffd9](https://www.jianshu.com/p/39727dbaffd9)

一个网上的脚本：

```python
from PIL import Image

def arnold(infile: str, outfile: str = None, a: int = 1, b: int = 1, shuffle_times: int = 1, reverse: bool = False) -> None:
    """
    Arnold猫脸变换函数

    Parameters:
        infile - 输入图像路径
        outfile - 输出图像路径
        a - Anrold 变换参数
        b - Anrold 变换参数
        shuffle_times - 置乱次数
        reverse - 逆变换
    """
    inimg = Image.open(infile)
    width, height = inimg.size
    indata = inimg.load()
    outimg = Image.new(inimg.mode, inimg.size)
    outdata = outimg.load()

    for _ in range(shuffle_times):
        for x in range(width):
            for y in range(height):
                if reverse:
                    nx = ((a * b + 1) * x - a * y) % width
                    ny = (y - b * x) % height
                else:
                    nx = (x + a * y) % width
                    ny = (b * x + (a * b + 1) * y) % height
                outdata[ny, nx] = indata[y, x]
    
    outimg.save(outfile if outfile else "arnold_"+infile, inimg.format)

arnold("before.png", "encode.png", 9, 39, 1)
arnold("encode.png", "decode.png", 9, 39, 1, True)

```

通常给a b数据可能给n 

二进制数据/rgb数据转图片:

图像逆序：

```python
infile = 'int.png'
outfile = 'out.png'

with open(infile, "rb") as fin:
    with open(outfile, "wb") as fout:
        fout.write(fin.read()[::-1])

```

#### png
**宽高：**

**题目会通过修改文件的宽高数据位来隐藏一些信息，我们可以通过比对crc位得到正确的宽高值**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750225698908-b103c10e-eb2e-4201-bddb-c2d936fc6fa4.png)

这是一个修改过宽高的图片的截图，我们可以看到仅仅有一句话其他什么也没有

而当我们正确的修改宽高后就可以看到隐藏在右下角的flag值

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750225802383-8794f857-21e4-40da-a9f3-96f54a4f7b33.png)

通常遇到比例奇怪的图片我们都可以尝试手动修改宽高

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750225899833-a5bdd2ac-e35a-4715-a381-dd0c74de1eaa.png)

1 处即为 宽度数据 2 处为高度数据 圈起来的地方为crc数据

当尝试发现可能被修改宽高后可以使用python脚本检测是否修改了宽高并修复得到正确宽高的图片

```python
import binascii
import itertools
import os
import struct
import zlib
import click


@click.command()
@click.option("-f","--file", required=True,help="file path")

def png_hw(file):
    # 修复png
    def modify_file_hex(file, position, new_hex_value):
                            try:
                                with open(file, 'rb') as f:
                                    content = f.read()
                                    hex_content = binascii.hexlify(content).decode()
                                    new_hex_content = hex_content[:position] + new_hex_value + hex_content[48:]
                                    modified_content = binascii.unhexlify(new_hex_content)
                                    output_file = os.path.join(os.path.dirname(file),
                                                                    'png_h_w_' + os.path.basename(file))
                                    with open(output_file, 'wb') as out_f:
                                        out_f.write(modified_content)
                                    return output_file
                            except FileNotFoundError:
                                return "文件不存在"
    try:
        png_data = open(f'{file}', 'rb').read()
        if png_data[:6].hex() != '89504e470d0a':
            print(f'非png文件')
        else:
            crc32key = zlib.crc32(png_data[12:29])  
            re_crc32 = int(png_data[29:33].hex(), 16) # 原始crc32值
            width = struct.unpack('>i', png_data[16:20])[0]
            height = struct.unpack('>i', png_data[20:24])[0]
            print(f'文件宽度：{width}, 文件高度：{height}')
            if crc32key == re_crc32:  
                print('文件宽高正确')
            else:
                print('文件宽高不正确，正在爆破宽高')
                for i, j in itertools.product(range(4095),
                                                range(
                                                    4095)):  
                    data = png_data[12:16] + struct.pack('>i', i) + struct.pack('>i', j) + png_data[24:29]
                    crc32 = zlib.crc32(data)
                    if crc32 == re_crc32:  
                        position = 32  
                        def pad_to_eight(s):
                            while len(s) < 8:
                                s = '0' + s
                            return s
                        w_out = pad_to_eight(hex(i)[2:])
                        h_out = pad_to_eight(hex(j)[2:])
                        new_hex_value = w_out + h_out
                        output_path = modify_file_hex(file, position, new_hex_value)
                        if output_path:
                            print(f'文件输出在{output_path}')
                        else:
                            print(f'文件错误')
    except ValueError:
        print("文件 error")
if __name__ == "__main__":
    png_hw()
```

**运行：**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750226142647-a19ff46a-da10-497b-b656-08860b14c8d4.png)

**文件分离：**

**binwalk**

这工具kali自带，可以在虚拟机安装一个kali

kali: [https://www.kali.org/get-kali/#kali-virtual-machines](https://www.kali.org/get-kali/#kali-virtual-machines)

vm虚拟机：[https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion](https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion)

vm下载需要注册，注册好无法登录去这里的mydownloads

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750226832605-2f428c4a-0442-42ae-8d20-98bda2d2eab9.png)

**用法：**

```shell
binwalk -e filename
```

**foremost:**

> sudo apt install foremost -y  # 安装foremost
>

**用法：**

```shell
foremost -i filename -o outpath
```

**盲水印：**

**单图盲水印：可以使用如下软件**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750227659203-a6b9f18a-7544-452e-9fd8-5d823664dd31.png)

[**https://www.123912.com/s/f2HzTd-9cz03**](https://www.123912.com/s/f2HzTd-9cz03)**提取码:FHgq**

**还有一个java盲水印工具 **[**https://github.com/ww23/BlindWatermark**](https://github.com/ww23/BlindWatermark)

**java -jar BlindWatermark-v0.0.3-windows-x86_64-gpu.jar decode -c gakki-dct-text-ec.jpg gakki-dct-text-dc.jpg**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750228630153-63c0463d-99e7-40a1-8677-19e0ba88161f.png)

**双图盲水印：**

**工具github地址：**

[**https://github.com/chishaxie/BlindWaterMark#blindwatermark**](https://github.com/chishaxie/BlindWaterMark#blindwatermark)

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750228030031-36c0e674-96af-4199-844e-0bd2291f6c4d.png)

另一个gui化的[https://github.com/fire-keeper/BlindWatermark](https://github.com/fire-keeper/BlindWatermark)

lsb隐写：

在png图片中，包含256的三次方个颜色，即16777216种，人类的眼睛可以区分约1,000万种不同的颜色，剩下无法区分的颜色就有6777216

LSB隐写就是修改RGB颜色分量的最低二进制位也就是最低有效位（LSB），而人类的眼睛不会注意到这前后的变化，我们仅对RGB中的最低位进行修改，如当前像素位点最后一位修改成1,1，0.则上述RGB变成218->219：

上述变化很难用肉眼察觉到，而且每一个像素位点携带了一位信息，那么我们可以利用八个字节的最低位存储一个比特信息，而该比特信息则可以转化为ASCII字符，从而达到隐写信息的目的

**zsteg:**

> 安装：
>
> github地址 [https://github.com/zed-0xff/zsteg](https://github.com/zed-0xff/zsteg)
>
> gem install zsteg
>

**主要用来检测png的lsb隐写，wbstego**

**StegSolve:**

**同样可以查看lsb，可以查看jpg...**

**在遇到题目给两张图片的时候亦可以使用他进行双图xor等**

**IDAT 块:**

**查看idat块是否正确，是否有多余的，可能为别的图像的数据块**

```shell
pngcheck file
```

#### jpg
**<font style="color:rgb(22, 18, 9);">OurSecret隐写：</font>**

**<font style="color:rgb(22, 18, 9);">特征明显，有如下数据</font>**

```shell
9E 97 BA 2A 00 80 88 C9 A3 70 97 5B A2 E4 99 B8
C1 78 72 0F 88 DD DC 34 2B 4E 7D 31 7F B5 E8 70
39 A8 B8 42 75 68 71 91

```

有密码，可以无密码

**stegdetect:**

stegdetect.exe -t jopi -s 10.0 1.jpg

检测加密

**silenteye：**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750231191904-f3d178e3-76b7-4707-acff-2a99905bf82a.png)

**steghide：**

```bash
steghide extract -sf filename -p passwd
```

**<font style="color:rgb(44, 63, 81);">JPHS：</font>**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750231214798-d09b16fc-f243-48c2-aa00-529fd548a942.png)

**<font style="color:rgb(85, 85, 85);">outguess：</font>**

```bash
outguess -k "pass" -r 1.jpg flag.txt
#-k 密钥
#flag.txt 保存位置
```

**<font style="color:rgb(85, 85, 85);">pixeljihad：</font>**

**<font style="color:rgb(85, 85, 85);">在线：</font>**[**https://sekao.net/pixeljihad/**](https://sekao.net/pixeljihad/)

**F5-steganography:**

```bash
#有密码
java Extract 1.jpg -p passwd
#无密码
java Extract 1.jpg
#数据会放到F5文件夹的output.txt

```

**JPG宽高隐写:**

**因为jpg和png不同，无法爆破crc确定正确的宽高只能手动修改**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1750231409809-e60de58c-012e-46e8-becf-a4fd75b872ba.png)

#### bmp
**宽高：**

可以使用gimp修改

bmp文件头去掉

**<font style="color:rgb(36, 41, 47);background-color:#FFFFFF;">silenteye：同上面的jpg</font>**

**<font style="color:rgb(36, 41, 47);background-color:#FFFFFF;">wbStego4open: 同上</font>**

#### gif
**gif分离：**

```shell
convert flag.gif flag.png
```

**帧间隔：**

```bash
identify -format "%s %T \n" flag.gif 
```

#### ......

### 音视频隐写
[https://www.123912.com/s/f2HzTd-ZhL03](https://www.123912.com/s/f2HzTd-ZhL03)提取码:LCtD

#### wav
**<font style="color:rgb(36, 41, 47);">silenteye:</font>**

<font style="color:rgb(36, 41, 47);">可能是silenteye隐写,使用如同jpg，有密匙使用密匙解</font>

**<font style="color:rgb(36, 41, 47);">deepsound：</font>**

使用deepsound 打开，如果需要密码说明就是 deepsound 隐写，有密钥直接填入密钥解密即可

如果是 deepsound 隐写但没有密钥，这个时候就可有使用deepsound2john脚本获取wav文件的哈希值

然后用john爆破hash

用法: john 1.txt

> https://github.com/openwall/john/blob/bleeding-jumbo/run/deepsound2john.py
>

**sstv：**

工具：[https://github.com/colaclanth/sstv](https://github.com/colaclanth/sstv)

可以使用rx-sstv

也可以使用集成的工具

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1752725113336-51e85718-bce8-45c3-8c4e-38b9775ca8e3.png)

**<font style="color:rgb(22, 18, 9);">电话音分析(DTMF)：</font>**

<font style="color:rgb(22, 18, 9);">使用工具：dtmf2num.exe</font>

<font style="color:rgb(22, 18, 9);">用法：dtmf2num.exe xxx.wav</font>

**<font style="color:rgb(22, 18, 9);">Audacity：</font>**

<font style="color:rgb(22, 18, 9);">使用Audacity.exe打开查看是否有字符串等信息</font>

**<font style="color:rgb(22, 18, 9);">steghide：</font>**

<font style="color:rgb(22, 18, 9);">也可能是steghide</font>

<font style="color:rgb(22, 18, 9);">用法：</font>

```bash
steghide extract -sf filename -p passwd
```

#### mp3
**<font style="color:rgb(22, 18, 9);">mp3stego：</font>**

<font style="color:rgb(22, 18, 9);">工具地址：</font>[https://www.petitcolas.net/steganography/mp3stego/](https://www.petitcolas.net/steganography/mp3stego/)

用法：

> decode -X -P pass sound.mp3     
> -X 是提取出隐写的文件  
> pass是解密时需要的密码   
> sound.mp3是待处理的MP3文件  
> # mp3stego可以使用无密码进行隐写
>

**stegpy：**

```bash
stegpy 1.wav -p
```

**<font style="color:rgb(22, 18, 9);">DeEgger Embedder：</font>**

<font style="color:rgb(22, 18, 9);">地址：</font>[https://www.softpedia.com/get/Security/Encrypting/DeEgger-Embedder.shtml](https://www.softpedia.com/get/Security/Encrypting/DeEgger-Embedder.shtml)

### 文档类隐写

#### pdf
**嵌入文件：**

使用binwalk 或者 foremost

**<font style="color:rgb(36, 41, 47);">wbStego4open:</font>**

<font style="color:rgb(22, 18, 9);">使用</font><font style="color:rgb(36, 41, 47);">wbStego4open</font><font style="color:rgb(22, 18, 9);">带密钥</font>

**<font style="color:rgb(22, 18, 9);">有密码：</font>**

<font style="color:rgb(22, 18, 9);">使用pdfcrack爆破密码（Ubuntu: apt install pdfcrack）</font>

```bash
pdfcrack -f enc.pdf -w rockyou.txt
```

#### word
可能将文字隐藏，全选修改背景和字体颜色即可看到隐藏的

使用binwalk分离附加的文件

利用行距隐写将行距的不用转化为01解摩斯密码（如：<font style="color:rgb(22, 18, 9);">ISCC2023-汤姆历险记 </font>）

#### ppt
最常见的binwalk分离

#### excel
<font style="color:rgb(22, 18, 9);">使用记事本打开查找flag</font>

<font style="color:rgb(22, 18, 9);">查看单元格的不同，将不同的格分别转化为黑白格组成二维码</font>

<font style="color:rgb(22, 18, 9);">binwalk</font>

#### ......

### 文本类隐写

#### 零宽
零宽隐写是一种利用零宽度字符在文本中隐藏信息的技术，这些字符在视觉上不可见，但可以存储和传递隐秘信息。

可以使用在线网站：

[https://tool.bfw.wiki/tool/1695021695027599.html](https://tool.bfw.wiki/tool/1695021695027599.html)

[https://www.hanloth.cn/tool/zero-width-secret](https://www.hanloth.cn/tool/zero-width-secret)

或者集成工具：

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1752726462853-d166bc78-1150-4ae1-a05a-55c02deb39e8.png)

#### base隐写
**可以使用集成工具：**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1752726579560-89fc51c7-029d-43cd-acce-214b48528f67.png)

#### ......
**<font style="color:rgb(22, 18, 9);">snow隐写：</font>**

<font style="color:rgb(22, 18, 9);">SNOW.EXE -C -p password flag.txt </font>

**<font style="color:rgb(22, 18, 9);">垃圾邮件隐写(spammimic)：</font>**

<font style="color:rgb(22, 18, 9);">使用在线网站解密：</font>

[<font style="color:rgb(35, 118, 183);">https://www.spammimic.com/</font>](https://www.spammimic.com/)

**文字隐写：**

在线网站：

[https://toolshu.com/hide-text](https://toolshu.com/hide-text)

### ......

## 流量分析
使用Wireshark.exe打开直接搜索

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1752726760518-dc6ab77c-2709-4d3e-a171-cb3f24b4cee0.png)

或者导出文件

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1752726835375-1cb334d9-8019-40c9-886e-6faa7cb4fe46.png)

## 取证题分析
使用vol解析

## 压缩包题分析

### 伪加密

```python
ZIP伪加密是一种通过修改ZIP文件头部的加密标志位，使文件被识别为加密压缩包的技术。实际上，这种加密并不真正保护文件内容，因此被称为“伪加密”。以下是ZIP伪加密的原理及其处理方法。

ZIP文件结构与伪加密原理

一个ZIP文件通常由三个部分组成：

压缩源文件数据区：包含文件的实际数据。

压缩源文件目录区：记录文件的元信息。

压缩源文件目录结束标志：标记目录的结束。

在ZIP文件中，加密属性由“全局方式位标记”决定：

无加密：全局方式位标记为00 00。

伪加密：数据区的全局方式位标记为00 00，但目录区的标记被修改为09 00。

真加密：数据区和目录区的全局方式位标记均为09 00。

伪加密的核心在于修改目录区的标记，使其显示为加密状态，但实际数据并未加密。
```

直接使用集成工具

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1752727513475-9c47a687-f1b9-45fc-bd50-161b3b61c249.png)

### 爆破
**archpr:**

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1752727604255-934f859f-f00d-4df1-95d5-bbc13f0cf198.png)

### 明文爆破
也可使用上述工具

要求：

<font style="color:rgb(51, 51, 51);">至少已知明文的12个字节及偏移，其中至少8字节需要连续。</font>

<font style="color:rgb(51, 51, 51);">明文对应的文件加密方式为ZipCrypto Store</font>

**<font style="color:rgb(51, 51, 51);">bkcrack:</font>**

[https://github.com/kimci86/bkcrack](https://github.com/kimci86/bkcrack)

### crc爆破
<font style="color:rgb(22, 18, 9);">压缩包中文件比较小只有几字节</font>

<font style="color:rgb(22, 18, 9);">工具：</font>

[https://github.com/AabyssZG/CRC32-Tools](https://github.com/AabyssZG/CRC32-Tools)

[https://github.com/theonlypwner/crc32](https://github.com/theonlypwner/crc32)

### ......

# CRYPTO

## RSA

### RSA基础理论及加解密过程
工具集成了一些常见的rsa攻击方式 只需要了解相关攻击即可使用

![](https://cdn.nlark.com/yuque/0/2025/png/46821499/1753933177946-d2a90513-cc04-4aa2-be1f-53606026646e.png)

<font style="color:rgb(32, 33, 34);">对极大整数做</font>[<font style="color:rgb(51, 102, 204);">因数分解</font>](https://zh.wikipedia.org/wiki/%E5%9B%A0%E6%95%B0%E5%88%86%E8%A7%A3)<font style="color:rgb(32, 33, 34);">的难度决定了 RSA 算法的可靠性。换言之，对一极大整数做因数分解愈困难，RSA 算法愈可靠。假如有人找到一种快速因数分解的算法的话，那么用 RSA 加密的信息的可靠性就会极度下降。但找到这样的算法的可能性是非常小的。今天只有短的 RSA 钥匙才可能被强力方式破解。到2020年为止，世界上还没有任何可靠的攻击RSA算法的方式。只要其钥匙的长度足够长，用RSA加密的信息实际上是不能被破解的。</font>

维基百科：

[https://zh.wikipedia.org/wiki/RSA%E5%8A%A0%E5%AF%86%E6%BC%94%E7%AE%97%E6%B3%95](https://zh.wikipedia.org/wiki/RSA%E5%8A%A0%E5%AF%86%E6%BC%94%E7%AE%97%E6%B3%95)

python的简单实现：

```python
from Crypto.Util.number import getPrime, inverse, bytes_to_long, long_to_bytes

flag =  b'flag{RSA}'

# 生成1024位的素数p和q

p = getPrime(1024)
q = getPrime(1024)

# 计算n, e, phi, d和c
n = p * q

e = 65537

phi = (p - 1) * (q - 1)

assert GCD(e, phi) == 1, "该e不满足互素条件"

d = inverse(e, phi)

c = pow(bytes_to_long(flag), e, n)

m = pow(c, d, n)

print(f'n = {n}')
print(f'e = {e}')   
print(f'd = {d}')
print(f'c = {c}')
print(f'm = {long_to_bytes(m)}')
```

rsa题目常见的参数 

p 素数生成n

q 素数生成n

pq 是解题的关键 通常要求的参数

n 与e组成公钥

e 与n组成公钥

c 加密后的密文

phi n的欧拉 =(p-1)*(q-1) pq = n p+q pq -p -q +1 = pq - (p+q) + 1 

d  私钥 解题的关键

m 明文

通常题目会给 n e c 

我们可以根据这三个参数来判断使用那些攻击方式

一开始我们可以尝试分解N，如果n不大

[http://www.factordb.com/](http://www.factordb.com/)

这是一个记录了很多已经被分解的n的pq

我们也可以使用yafu分解，如果pq相差较大或小的时候，可以根据题目所给加密代码判断

[https://sourceforge.net/projects/yafu/](https://sourceforge.net/projects/yafu/)

我们还需要学习一些python库

Crypto

gmpy2

### 常见攻击方式

#### <font style="color:rgb(0, 0, 0);">小明文攻击</font>
当题目中N特别大的时候可以尝试

我们已知 Ⅰ:  C  <font style="color:rgb(0, 0, 0);">≡</font>![image](https://cdn.nlark.com/yuque/__latex/cc221ed71b2d6a5f6487c0d93be71c3d.svg)<font style="color:rgb(0, 0, 0);">(mod N)</font>

<font style="color:rgb(0, 0, 0);">当m很小的时候 m的e次方小于n</font>

<font style="color:rgb(0, 0, 0);">所以 c 就等于 m的e次方 此时我们只要将 c 开 e 次方就可以得到 m</font>

<font style="color:rgb(0, 0, 0);">这里使用 gmpy2 库的iroot开方</font>

```python
from Crypto.Util.number import *
from gmpy2 import *
n  = 536410484994483033093334003836655729325470269375524009439921349251765426879326472420715343135213685847853149465047363004844978980705334818310367627899054282724091430760574321302693735313741776534635308880108579425210969875273787315835179223662471838419622222586196334875552681127482220681804218077447446727632367288719418398225173584249649494060944903031644643599350735559974998992685357629587918116319437983541031003274274249512385723959144711034887286740398048911255492577006594659820438597055144909808217806214389981467817007584648955570726162669186034727073111376869516381199706615431972535815322666741187757365776611420640881256943303112723909875163327558585208160248953717008905206187852681531673607531360656420914879152163720617911529983435735678874123738624814506966909449518581239944997840945458848686624613184987748822188025864390108649415309566456540845277892075600527410134107469406816659137099034223840641145291291677316961839250222786771084598108203101897949775024306470936804403534408830935782941709356062377127100322538567707179546810871854386057481906331948667458888491116697493079241029509563403449393692443545157249665866189068291745976311888965264882340009888119575540460672793226773934767675512684750592502994661
e = 47
c = 229899396883582392364871905906445296949203163435377967308523386636507105732351552139686055293875453912112843930875659740397422297275613832964886182478284228932337946906215427434632071627272673570051303664678550765869183098488754645162034875760803916176659931431903280877040008151839312486086810338837714295821068677830038145047288362507454852643283361570635475479731085221630599511037989875119938896391192076787426053096532792131784563523065082875308622036981017576697767085294161885999051064464805324234829382111945083257918268260979566515252826957333562648074716098524243209378279602403795364197351006272703919005850152191380237640254523031072133802051271379417062521178212883200712566363108988562038188056490055724405896019781505695009412712690784013380990981185039802898643638127923786296260202685639474550000877637714438089700174399902960859666510114240835250541384360368049671274643421485904308653603924744567918821295775350084960806905039253932125210810019431964659889918601526879604439206186643987785399968027152305034576184766368079201408412844596024313611950909884330051927770353597750655703028328638756559133666564620074677469304330050449745861462898383722361080035329755112868572844306365995005218909407333254086037  

m = iroot(c, e)

print(long_to_bytes(m[0]))
```

#### <font style="color:rgb(0, 0, 0);">低加密指数攻击</font>
由 Ⅰ 消去模 得到 ![image](https://cdn.nlark.com/yuque/__latex/5408886ac0518174dec52ede9a1a5951.svg)= c + k*n

当e很小的时候 我们可以爆破k 得到正确的 ![image](https://cdn.nlark.com/yuque/__latex/5408886ac0518174dec52ede9a1a5951.svg)

```python
from Crypto.Util.number import *
from gmpy2 import *
n = 25066689877776679233022203369122860358311144108034322786249336304184718167290635002070039262490792542129164733263246201499413220464411226682235152645481523633440451076347588502189820875766207732385081347542902014379448935897761402426197951109899225264278881605284920398145164965059125758041113782043
e = 5
c = 9580937997026657207695606535792321409809664111257153374644767194117132680120146044970386750643915697649050660680091489013318267184823888266207920970701381149337870449324937658700572686851552653818796958133992739190614740958850104564209920508542730206551286453342339610980738869413911612550009452577
for k in range(100000):
    me = c + k*n
    res = iroot(me, e) # iroot返回 一个元组，第一个元素是整数的整数根，第二个元素是布尔值，表示是否是整数根
    if res[1]:
        m = res[0]
        break
print(long_to_bytes(m))
```

#### <font style="color:rgb(0, 0, 0);">Rabin算法攻击</font>
一个显著的特征 e为2

```python
from Crypto.Util.number import *
from gmpy2 import *

p = 
q = 
e = 2
c = 

def rabin_attack(c, n, p, q):
    c1 = powmod(c, (p+1)//4, p)
    c2 = powmod(c, (q+1)//4, q)
    cp1 = p - c1
    cp2 = q - c2

    t1 = invert(p, q)
    t2 = invert(q, p)

    m1 = (q*c1*c2 + p*c2*t1) % n
    m2 = (q*c1*t2 + p*cp2*t1) % n
    m3 = (q*cp1*t2 + p*c2*t1) % n
    m4 = (q*cp1*t2 + p*cp2*t1) % n

    return m1, m2, m3, m4

ms = rabin_attack(c, p*q, p, q)

for m in ms:
    print(long_to_bytes(m))
```

#### <font style="color:rgb(0, 0, 0);">Wiener攻击</font>
[https://github.com/pablocelayes/rsa-wiener-attack](https://github.com/pablocelayes/rsa-wiener-attack)

```python
from Crypto.Util.number import *
from gmpy2 import *

n = 
e = 
c = 

class ContinuedFraction():
    def __init__(self, numerator, denumerator):
        self.numberlist = []  
        self.fractionlist = []  
        self.GenerateNumberList(numerator, denumerator)
        self.GenerateFractionList()

    def GenerateNumberList(self, numerator, denumerator):
        while numerator != 1:
            quotient = numerator // denumerator
            remainder = numerator % denumerator
            self.numberlist.append(quotient)
            numerator = denumerator
            denumerator = remainder

    def GenerateFractionList(self):
        self.fractionlist.append([self.numberlist[0], 1])
        for i in range(1, len(self.numberlist)):
            numerator = self.numberlist[i]
            denumerator = 1
            for j in range(i):
                temp = numerator
                numerator = denumerator + numerator * self.numberlist[i - j - 1]
                denumerator = temp
            self.fractionlist.append([numerator, denumerator])


a = ContinuedFraction(e, n)
for k, d in a.fractionlist:
    m = powmod(c, d, n)
    flag = long_to_bytes(m)
    
    if b'flag' in flag:  #根据具体的flag头更改
        print(flag)
```

#### <font style="color:rgb(0, 0, 0);">低加密指数广播攻击</font>
<font style="color:rgb(51, 51, 51);">当有多组n，c的时候，且e小</font>

```python
import libnum
from gmpy2 import invert, gcd, iroot

def op(x):
    res = 1
    for i in x:
        res *= i
    return res

def CRT(m, a):
    assert (len(m) == len(a))
    M = op(m)
    sum = 0
    for m, a in zip(m, a):
        Mi = M // m
        ti = invert(Mi, m)
        sum += a * ti * Mi
    return sum % M
def GCRT(m, a):
    assert (len(m) == len(a))
    curm, cura = m[0], a[0]
    for m, a in zip(m[1:], a[1:]):
        d = gcd(curm, m)
        c = a - cura
        assert (c % d == 0)
        K = c // d * invert(curm // d, m // d)
        cura += curm * K
        curm = curm * m // d
    return cura % curm

e= 23
n= [, , , , , , ]
c= [, , , , , , ]

m = CRT(n, c)
m1 = iroot(m, e)  # 开e次方
print(m1)
print(libnum.n2s(int(m1[0])))
```

#### <font style="color:rgb(0, 0, 0);">p-1光滑攻击</font>
<font style="color:rgb(51, 51, 51);">光滑数：指可以分解为小素数乘积的正整数</font>

```python
from Crypto.Util.number import *
from gmpy2 import *
n =
e = 65537
c = 
a = 2
m = 2
while True:
    a = powmod(a, m, n)
    p = gcd(a-1, n)
    if p != 1 and p != n:
        break
    m += 1
print(p)
q = n // p

phi = (p-1)*(q-1)
d = invert(e, phi)
m = powmod(c, d, n)
print(long_to_bytes(m))
```

#### <font style="color:rgb(0, 0, 0);">p+1光滑攻击</font>

```python
from Crypto.Util.number import *
from gmpy2 import *
from itertools import count

n = 
e = 65537
c = 

def mlucas(v, a, n):
    v1, v2 = v, (v ** 2 - 2) % n
    for bit in bin(a)[3:]: v1, v2 = ((v1 ** 2 - 2) % n, (v1 * v2 - v) % n) if bit == "0" else (
        (v1 * v2 - v) % n, (v2 ** 2 - 2) % n)
    return v1

def primegen():
    yield 2
    yield 3
    yield 5
    yield 7
    yield 11
    yield 13
    ps = primegen()  # yay recursion
    p = ps.__next__() and ps.__next__()
    q, sieve, n = p ** 2, {}, 13
    while True:
        if n not in sieve:
            if n < q:
                yield n
            else:
                next, step = q + 2 * p, 2 * p
                while next in sieve:
                    next += step
                sieve[next] = step
                p = ps.__next__()
                q = p ** 2
        else:
            step = sieve.pop(n)
            next = n + step
            while next in sieve:
                next += step
            sieve[next] = step
        n += 2

def ilog(x, b):  # greatest integer l such that b**l <= x.
    l = 0
    while x >= b:
        x /= b
        l += 1
    return l

def attack(n):
    for v in count(1):
        for p in primegen():
            e = ilog(isqrt(n), p)
            if e == 0:
                break
            for _ in range(e):
                v = mlucas(v, p, n)
            g = gcd(v - 2, n)
            if 1 < g < n:
                return int(g), int(n // g)  # g|n
            if g == n:
                break

p, q = attack(n)


phi = (p-1)*(q-1)
d = invert(e, phi)
m = powmod(c, d, n)
print(long_to_bytes(m))
```

#### <font style="color:rgb(0, 0, 0);">共模攻击</font>
题目给出两对e c 公用同一个n

```python
from gmpy2 import *
from Crypto.Util.number import *

n = 

e1 = 
e2 = 

c1 = 
c2 = 

_, s1, s2 = gcdext(e1, e2)

m = powmod(c1, s1, n) * powmod(c2, s2, n) % n
print(long_to_bytes(m))
```

#### <font style="color:rgb(0, 0, 0);">dp&dq泄露攻击</font>

```python
import gmpy2
import libnum
def decrypt(dp,dq,p,q,c):
    InvQ = gmpy2.invert(q, p)
    mp = pow(c, dp, p)
    mq = pow(c, dq, q)
    m = (((mp-mq)*InvQ) % p)*q+mq
    print(libnum.n2s(int(m)).decode())
p= 
q= 
dq= 
dp= 
c= 
decrypt(dp,dq,p,q,c) 
```

#### <font style="color:rgb(0, 0, 0);">dp泄露攻击</font>

```python
import libnum
import gmpy2
n= 
e= 65537
dp= 
c= 
for i in range(1,65535):
    p=(dp*e-1)//i+1
    if n%p==0:
        q=n//p
        break
phi_n= (p-1)*(q-1)
d=gmpy2.invert(e,phi_n)
m=pow(c,d,n)
print(m)
flag=libnum.n2s(int(m)).decode()
print(flag)
```

#### <font style="color:rgb(0, 0, 0);">e很大的dp泄露攻击</font>

```python
from Crypto.Util.number import *
from gmpy2 import *

n = 
e = 
c = 
dp = 

m = #随机
p = gcd(powmod(m, e*dp, n) - m, n)
q = n // p
d = invert(e, (p - 1) * (q - 1))
m = powmod(c, d, n)
print(long_to_bytes(m))
```

#### <font style="color:rgb(0, 0, 0);">已知明文高位攻击</font>
需要sage

[https://mirrors.aliyun.com/sagemath/win/index.html](https://mirrors.aliyun.com/sagemath/win/index.html)

m高位已知

```python
import libnum
def phase2(high_m, n, c):
    R.<x> = PolynomialRing(Zmod(n), implementation='NTL')
    m = high_m + x
    M = m((m^3 - c).small_roots()[0])
    print(libnum.n2s(int(M)))
n= 
e= 3
c= 
high_m= 

phase2(high_m, n, c) 
```

#### <font style="color:rgb(0, 0, 0);">已知p高位攻击</font>
需要sage

```python
n = 
p4=
e = 0x10001
pbits = 1024
kbits = pbits - p4.nbits()
print(p4.nbits())
p4 = p4 << kbits
PR.<x> = PolynomialRing(Zmod(n))
f = x + p4
roots = f.small_roots(X=2^kbits, beta=0.4)
if roots:
    p = p4+int(roots[0])
    print (n)
    print (p)
    print (n/p)
```

#### <font style="color:rgb(0, 0, 0);">AMM算法</font>
好文章[https://xz.aliyun.com/news/13908](https://xz.aliyun.com/news/13908)

```python

from Crypto.Util.number import *
from gmpy2 import *
import random
import math

n = 
c = 
p =    
q = 
e = 

def onemod(e, q):
    p = random.randint(1, q-1)
    while(powmod(p, (q-1)//e, q) == 1):  # (r,s)=1
        p = random.randint(1, q)
    return p

def AMM_rth(o, r, q):  # r|(q-1
    assert((q-1) % r == 0)
    p = onemod(r, q)

    t = 0
    s = q-1
    while(s % r == 0):
        s = s//r
        t += 1
    k = 1
    while((s*k+1) % r != 0):
        k += 1
    alp = (s*k+1)//r

    a = powmod(p, r**(t-1)*s, q)
    b = powmod(o, r*a-1, q)
    c = powmod(p, s, q)
    h = 1

    for i in range(1, t-1):
        d = powmod(int(b), r**(t-1-i), q)
        if d == 1:
            j = 0
        else:
            j = (-math.log(d, a)) % r
        b = (b*(c**(r*j))) % q
        h = (h*c**j) % q
        c = (c*r) % q
    result = (powmod(o, alp, q)*h)
    return result

def ALL_Solution(m, q, rt, cq, e):
    mp = []
    for pr in rt:
        r = (pr*m) % q
        # assert(pow(r, e, q) == cq)
        mp.append(r)
    return mp


def calc(mp, mq, e, p, q):
    i = 1
    j = 1
    t1 = invert(q, p)
    t2 = invert(p, q)
    for mp1 in mp:
        for mq1 in mq:
            j += 1
            if j % 100000 == 0:
                print(j)
            ans = (mp1*t1*q+mq1*t2*p) % (p*q)
            if check(ans):
                return
    return


def check(m):
    try:
        a = long_to_bytes(m)
        if b'NSSCTF' in a:
            print(a)
            return True
        else:
            return False
    except:
        return False


def ALL_ROOT2(r, q):  # use function set() and .add() ensure that the generated elements are not repeated
    li = set()
    while(len(li) < r):
        p = powmod(random.randint(1, q-1), (q-1)//r, q)
        li.add(p)
    return li

cp = c % p
cq = c % q

mp = AMM_rth(cp, e, p)  # AMM算法得到一个解
mq = AMM_rth(cq, e, q)

rt1 = ALL_ROOT2(e, p)  # 得到所有的ri，即(ri*mp)^e%p = 1
rt2 = ALL_ROOT2(e, q)

amp = ALL_Solution(mp, p, rt1, cp, e)  # 得到所有的mp
amq = ALL_Solution(mq, q, rt2, cq, e)

calc(amp, amq, e, p, q)  # 俩俩CRT
```

#### <font style="color:rgb(51, 51, 51);">剪枝</font>
<font style="color:rgb(51, 51, 51);">a1^b1：</font>

```python
from Crypto.Util.number import *
import sys

sys.setrecursionlimit(1500)

# part1,剪枝
a1 = 
b1 = 
c1 = 
e = 65537
a1 = "0" + str(bin(a1)[2:])


def find(p, q):
    l = len(p)
    tmp0 = p + (1024 - l) * "0"
    tmp1 = p + (1024 - l) * "1"
    tmq0 = q + (1024 - l) * "0"
    tmq1 = q + (1024 - l) * "1"
    if (int(tmp0, 2) < int(tmq0, 2)):
        return
    if (int(tmp0, 2) * int(tmq0, 2) > b1):
        return
    elif (int(tmp1, 2) * int(tmq1, 2) < b1):
        return

    if (l == 1024):
        pp = int(tmp0, 2)
        qq = int(tmq0, 2)
        d = inverse(e, (pp - 1) * (qq - 1))
        m = long_to_bytes(pow(c1, d, pp * qq))
        print(str(m)[2:-1], end="")

    else:
        if (a1[l] == "1"):
            find(p + "1", q + "0")
            find(p + "0", q + "1")
        else:
            find(p + "0", q + "0")
            find(p + "1", q + "1")


tempp = ""
tempq = ""
find(tempp, tempq)
```

<font style="color:rgb(51, 51, 51);">p ^ _q：</font>

<font style="color:rgb(51, 51, 51);">p与q的反方向二进制的异或值</font>

```python
from Crypto.Util.number import *
import sys
sys.setrecursionlimit(1500)

pxorq = 
n =
c = 
e = 65537
pxorq = str(bin(pxorq)[2:]).zfill(256)
 
def find(ph,qh,pl,ql):
    l = len(ph)
    tmp0 = ph + (256-2*l)*"0" + pl
    tmp1 = ph + (256-2*l)*"1" + pl
    tmq0 = qh + (256-2*l)*"0" + ql
    tmq1 = qh + (256-2*l)*"1" + ql
    if(int(tmp0,2)*int(tmq0,2) > n):
        return 
    if(int(tmp1,2)*int(tmq1,2) < n):
        return
    if(int(pl,2)*int(ql,2) % (2**(l-1)) != n % (2**(l-1))):
        return

    if(l == 128):
        pp0 = int(tmp0,2)
        if(n % pp0 == 0):
            pf = pp0
            qf = n//pp0
            phi = (pf-1)*(qf-1)
            d = inverse(e,phi)
            m1 = pow(c,d,n)
            print(long_to_bytes(m1))
            exit()

    else:
        if(pxorq[l] == "1" and pxorq[255-l] == "1"):
            find(ph+"1",qh+"0","1"+pl,"0"+ql)
            find(ph+"0",qh+"0","1"+pl,"1"+ql)
            find(ph+"1",qh+"1","0"+pl,"0"+ql)
            find(ph+"0",qh+"1","0"+pl,"1"+ql)
        elif(pxorq[l] == "1" and pxorq[255-l] == "0"):
            find(ph+"1",qh+"0","0"+pl,"0"+ql)
            find(ph+"0",qh+"0","0"+pl,"1"+ql)
            find(ph+"1",qh+"1","1"+pl,"0"+ql)
            find(ph+"0",qh+"1","1"+pl,"1"+ql)
        elif(pxorq[l] == "0" and pxorq[255-l] == "1"):
            find(ph+"0",qh+"0","1"+pl,"0"+ql)
            find(ph+"0",qh+"1","0"+pl,"0"+ql)
            find(ph+"1",qh+"0","1"+pl,"1"+ql)
            find(ph+"1",qh+"1","0"+pl,"1"+ql)
        elif(pxorq[l] == "0" and pxorq[255-l] == "0"):
            find(ph+"0",qh+"0","0"+pl,"0"+ql)
            find(ph+"1",qh+"0","0"+pl,"1"+ql)
            find(ph+"0",qh+"1","1"+pl,"0"+ql)
            find(ph+"1",qh+"1","1"+pl,"1"+ql)

find("1","1","1","1")
```

## <font style="color:rgb(79, 79, 79);">DSA</font>

### 原理及加解密过程
[https://zh.wikipedia.org/wiki/%E6%95%B0%E5%AD%97%E7%AD%BE%E5%90%8D%E7%AE%97%E6%B3%95](https://zh.wikipedia.org/wiki/%E6%95%B0%E5%AD%97%E7%AD%BE%E5%90%8D%E7%AE%97%E6%B3%95)

## <font style="color:rgb(79, 79, 79);">ECC</font>

### 原理及加解密过程

## <font style="color:rgb(79, 79, 79);">AES/DES</font>

## ......

## 脚本:

```python
#!/bin/bash
# 作为misc的通用tools
# huihuilikaile 20250425



# 设置颜色信息
# 基本文字颜色
BLACK_TEXT="\033[30m"
RED_TEXT="\033[31m"
GREEN_TEXT="\033[32m"
YELLOW_TEXT="\033[33m"
BLUE_TEXT="\033[34m"
PURPLE_TEXT="\033[35m"
CYAN_TEXT="\033[36m"
WHITE_TEXT="\033[37m"

# 基本背景颜色
BLACK_BG="\033[40m"
RED_BG="\033[41m"
GREEN_BG="\033[42m"
YELLOW_BG="\033[43m"
BLUE_BG="\033[44m"
PURPLE_BG="\033[45m"
CYAN_BG="\033[46m"
WHITE_BG="\033[47m"

# 亮色文字颜色
BRIGHT_BLACK_TEXT="\033[1;30m"
BRIGHT_RED_TEXT="\033[1;31m"
BRIGHT_GREEN_TEXT="\033[1;32m"
BRIGHT_YELLOW_TEXT="\033[1;33m"
BRIGHT_BLUE_TEXT="\033[1;34m"
BRIGHT_PURPLE_TEXT="\033[1;35m"
BRIGHT_CYAN_TEXT="\033[1;36m"
BRIGHT_WHITE_TEXT="\033[1;37m"

# 自定义 RGB 颜色
CUSTOM_RED_TEXT="\033[38;2;255;0;0m"
CUSTOM_GREEN_BG="\033[48;2;0;255;0m"

# 组合背景颜色

GREEN_WHITE_TEXT="\033[1;47;32m"
BLUE_WHITE_TEXT="\033[1;34;47m"
BLUE_GREE_TEXT="\033[34;42m"
# 重置颜色
RESET="\033[0m"

# 设置颜色函数

RED_B() {
    echo "${RED_TEXT}${1}${RESET}\n"
}

BLUE_B() {
    echo "${BLUE_TEXT}${1}${RESET}\n"
}

RED_LB() {
    echo "${BRIGHT_RED_TEXT}${1}${RESET}\n"
}

BLUE_LB() {
    echo "${BRIGHT_BLUE_TEXT}${1}${RESET}\n"
}

ALL_B() {
    echo "${BLUE_WHITE_TEXT}${1}${RESET}\n"
}

BLUE_GREE_B() {
    echo "${BLUE_GREE_TEXT}${1}${RESET}\n"
}

FENGE() {
    echo "${GREEN_TEXT}${1}${RESET}\n"
}

# 设置帮助信息
usage() {
    echo "Usage: $0 [-f <arg>] [-p <arg>] [-j <arg>] [-g <arg>] [-h]"
    echo "  -f filename  提供文件的类型,EXIF,关键字检测,文件隐藏(binwalk foremost)等信息"
    echo "  -p True/T/t  进行png相关的检测 "
    echo "  -j key  进行jpg相关的检测 "
    echo "  -g True/T/t  进行gif相关的检测 "
    echo "  -h 获取帮助"
    exit 1
}


# ANSI 转义码定义
RED='\033[0;31m'
GREEN='\033[0;32m'
YELLOW='\033[0;33m'
BLUE='\033[0;34m'
NC='\033[0m' # 重置颜色

# 函数：将文本添加带颜色的边框
add_colored_border() {
  local text="$1"
  local length=${#text}
  
  # 计算边框宽度（增加一些额外的空间）
  local border_width=$((length + 4))
  
  # 打印上边框
  printf "${BLUE_TEXT}+%0.s-" $(seq 1 $border_width)
  echo "--${NC}"
  
  # 打印文本行
  printf "${colBLUE_TEXTor} %s ${NC}\n" "$text"
  
  # 打印下边框
  printf "${BLUE_TEXT}+%0.s-" $(seq 1 $border_width)
  echo "--${NC}"
}

# 关键字

CHARKEY="flag|FLAG|pass|pk|PK|Pk|ctf|CTF|KEY|key|txt|PASS"

# 目录设置

binwalkout="binwalkoutfile"

foremostout="foremostoutfile"

# 字符匹配函数
grep_file() {
    outkeys=$(strings "${1}" | grep "-E" "${CHARKEY}")
    add_colored_border $outkeys
}
# 文件类型匹配
file_type() {
    file $1
}

# exif数据
exif_file() {
    exiftool "$1"
}



forf() {
    timefile=$(date +"%H%M%S")
    filename="${foremostout}/${timefile}_${1%%.*}"
    if [ -d $filename ]; then
        RED_LB "${RED_TEXT}目录${filename}不为空,重新创建:${RESET}"
        timefile=$(date +"%H%M%S")
        filename="${foremostout}/${timefile}_${1%%.*}"
        mkdir $filename
        BLUE_LB "新目录:${filename}"
        foremost "-i" "$1" "-o" "${filename}"
        FENGE "目录树: "
        tree $filename
    else
        mkdir $filename
        
        foremost "-i" "$1" "-o" "${filename}"

        BLUE_LB "\nforemost输出目录: ${filename}"

        FENGE "目录树: "
        tree $filename
    fi
}
#------------------图片相关---------------------
# OurSecret隐写检测
OurSecret_file() {
    # 模拟 xxd 输出
    xxd_output=$(xxd "-p" $1)

    # 待比对的十六进制数据
    target_hex="9e97ba2a008088c9a370975ba2e499b8c178720f88dddc342b4e7d317fb5e87039a8b84275687191"

    # 进行比对
    if echo "$xxd_output" | grep -q "$target_hex"; then
        RED_B "可能存在OurSecret"
    else
        BLUE_LB "不存在OurSecret隐写"
    fi
}


# 设置参数选项
while getopts ":f:p:j:g:b:h" opt; do
    case $opt in
        f)
            # BINWALK FOREMOST STRINGS GREP
            FENGE "-----------------信息收集-------------------"
            BLUE_GREE_B "文件类型检测:"
            file_type $OPTARG
            BLUE_GREE_B "关键字:"
            grep_file $OPTARG
            BLUE_GREE_B "exif数据:"
            exif_file $OPTARG
            BLUE_GREE_B "FOREMOST 分离结果:"
            forf $OPTARG
            f_name="$OPTARG"
            
            ;;
        p)
            PTRUE=true
            FENGE "-----------------PNG相关检测-------------------"
            BLUE_GREE_B "png宽高检测:"
            pnghwout=$(python3 "pnghw.py" "-f" "${f_name}")
            BLUE_LB $pnghwout
            BLUE_GREE_B "png IDAT快检测:"
            pngcheck "-v" "${f_name}"
            
            BLUE_GREE_B "OurSecret隐写检测:"
            OurSecret_file $f_name
            ;;
        j)
            BLUE_GREE_B "OurSecret隐写检测:"
            OurSecret_file $f_name
            BLUE_GREE_B "steghide未知密码隐写检测:"
            steghide "extract" "-sf" $f_name
            BLUE_GREE_B "outguess隐写检测:"
            outguess "-k" "$OPTARG" "-r"  $f_name "${f_name%%.*}.txt"
            BLUE_LB "输出文件为：${f_name%%.*}.txt"
            ;;
        g)
            BLUE_B "Option c$OPTARG"
            ;;
        g)
            BLUE_B "Option c$OPTARG"
            ;;
	    h)
	        usage
	        ;;
        \?)
            RED_LB "未知选项: -$OPTARG" >&2
            ;;
        :)
            RED_LB "提供给 -$OPTARG 选项一个参数." >&2
            ;;
    esac
done 
FENGE "-----------------储存资料-------------------"
cat "www.txt"
if [ "$PTRUE" = true ]; then
    BLUE_GREE_B "执行zsteg: "
    zsteg "-a" "$f_name"
fi

```

