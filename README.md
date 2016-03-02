# 概述
**translate** - 这个程序使用 [Glosbe](https://glosbe.com/#) 提供的 [API](https://glosbe.com/a-api),在能够连接到因特网的情况下，可以在 Linux 终端下实现英文单词到中文的翻译和中文单词到英文的翻译。         

# 用法格式          
**translate** [**-h**] [**-v** | **-q**] [**-e** | **-z**] _word_

# 描述             
这个程序使用 [Glosbe](https://glosbe.com/#) 提供的 [API](https://glosbe.com/a-api),在能够连接到因特网的情况下，可以在 Linux 终端下实现英文单词到中文的翻译和中文单词到英文的翻译。            

## 选项            
**-h**, **--help**          
&nbsp;&nbsp;&nbsp;&nbsp;查看帮助                
**-v**, **--verbose**          
&nbsp;&nbsp;&nbsp;&nbsp;详细地输出翻译的结果                
**-q**, **--quiet**            
&nbsp;&nbsp;&nbsp;&nbsp;简略地输出翻译的结果(默认选项)               
**-e**, **--english**              
&nbsp;&nbsp;&nbsp;&nbsp;要翻译的单词为英文(默认选项)                  
**-z**, **--chinese**              
&nbsp;&nbsp;&nbsp;&nbsp;要翻译的单词为中文(默认选项)            

# 如何使用这个程序?
首先使用 **root** 身份或权限执行如下命令:               

\# **mv** -v ./translate /usr/bin/             
\# **chown** *your_username:your_username* /usr/bin/translate         

如果使用的是 **Ubuntu**, 可以直接执行如下命令:               

```bash
$ make
```

## 一些例子               

将英文 **`dog`** 翻译成中文:          

```bash         
$ translate -e dog     
```            
或者是                 

```bash
$ translate dog      # -e 为默认选项
```            
将英文 **`dog`** 翻译成中文，并且查看翻译的详细输出:                 

```bash
$ translate -v dog
```             
将中文 **`苹果`** 翻译成英文:                 

```bash
$ translate -z 苹果            
```
