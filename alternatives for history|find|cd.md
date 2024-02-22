<i>The most commonly used commands when navigating are `history`, `find`, `cd`. Here are some examples of simple alternative tools that does a better job.</i>

<details><summary><b>Easily view, navigate, search history commands</b> <img src="https://user-images.githubusercontent.com/18756975/201506874-0dd9a164-0b81-45fe-9c91-63122dcec9b8.PNG" width=20px height=20px></summary>

[htsr](https://github.com/dvorka/hstr)<br>
![hts](https://user-images.githubusercontent.com/18756975/201403803-7f899124-3412-443c-9b6d-e60b8b2ca889.png)<br>
_**Install**_ :
```bash
sudo apt install hstr -y && hstr --show-configuration >> ~/.bashrc
```
_Restart terminal_
> **Note** - Other installation info - [github.com/dvorka/hstr/blob/master/INSTALLATION.md](https://github.com/dvorka/hstr/blob/master/INSTALLATION.md#installation)

**_Usage_** :
```bash
hstr keyword
```
Interactive searching🔎 :
`Ctrl+R`

>**Note** - More info on usage :

>     man hstr
#

</p>
 </details>


<details><summary><b>A simple and userfriendly way to find files</b> <img src="https://user-images.githubusercontent.com/18756975/201507256-a36e655d-66b0-4851-a035-6c87b10d7f1e.PNG" width=16px height=20px></summary>

<p align="center">
<a href="https://github.com/sharkdp/fd"><b>fd</b></a> and <a href="https://github.com/junegunn/fzf"><b>fzf</b></a><br>
<img src="https://user-images.githubusercontent.com/18756975/201507691-6dce9975-1abd-4fac-b347-f8f6ba2654e6.svg" width=400px height=300px><img src="https://user-images.githubusercontent.com/18756975/202026845-bdb69d8e-0500-4748-8cd6-bc0ba4d019a7.png" width=400px height=300px>


_**Install**_ :
```bash
sudo apt install fd-find -y && sudo apt install fzf -y  
```
_**Add binary link**_<i>(set correct bin directory location if error)</i> :
```bash
ln -s $(which fdfind) ~/.local/bin/fd
```
_Restart terminal_
> **Note** - Other installation info : <br>
[github.com/sharkdp/fd#installation](https://github.com/sharkdp/fd#installation)<br>
[github.com/junegunn/fzf#installation)](https://github.com/junegunn/fzf#installation)

_**Usage**_ :

<table class="tg">
<tbody>
<tr>
<th align=left class="tg-yw4l">Command</th>
<th class="tg-yw4l">Description</th>
</tr>
<tr>
<td align=left class="tg-yw4l">fd foo</td>
<td class="tg-yw4l">Find in current directory, the string pattern name "foo", in parent|sub directories and files.</td>
</tr>
 <tr>
<td align=left class="tg-yw4l">fd foo /FOO2</td>
<td class="tg-yw4l">Find in "FOO2" directory, the string pattern name "foo", in parent|sub directories and files.</td>
</tr>
<tr>
<td align=left class="tg-yw4l">fd -g|--glob foo /FOO2</td>
<td class="tg-yw4l">Find in "FOO2" directory, the <a href="https://www.google.com/search?q=What+is+glob+used+for+%3F&client=firefox-b-d&sxsrf=ALiCzsZ01R6o0gluLQgsslLDYABmC3jhcQ%3A1668511191028&ei=13VzY4KrAa3m5NoPgrCxwAw&ved=0ahUKEwjC8uDGiLD7AhUtM1kFHQJYDMgQ4dUDCA4&uact=5&oq=What+is+glob+used+for+%3F&gs_lcp=Cgxnd3Mtd2l6LXNlcnAQAzIHCCMQsAMQJzIKCAAQRxDWBBCwAzIKCAAQRxDWBBCwAzIKCAAQRxDWBBCwAzIKCAAQRxDWBBCwAzIKCAAQRxDWBBCwAzIKCAAQRxDWBBCwAzIKCAAQRxDWBBCwAzIKCAAQRxDWBBCwA0oECE0YAUoECEEYAEoECEYYAFAAWABgwgFoAXABeACAAQCIAQCSAQCYAQDIAQnAAQE&sclient=gws-wiz-serp"><b>glob</b></a> pattern name <i>matching</i> "foo", in parent|sub directories and files.</td>
</tr>
 <tr>
<td align=left class="tg-yw4l">fd /foo -p|--path /FOO2</td>
<td class="tg-yw4l">Find in "FOO2" directory and view the files and directory paths and its contents that is or starts with the string pattern name "foo".</td>
</tr>
 <tr>
<td align=left class="tg-yw4l">fd foo/ -p|--path /FOO2</td>
<td class="tg-yw4l">Find in "FOO2" directory and view the directory paths and its contents that is or ends with the string pattern name "foo".</td>
</tr>
<tr>
<td align=left class="tg-yw4l">fd -t|--type -d foo</td>
<td class="tg-yw4l">Find for directory type only.</td>
</tr>
 <tr>
<td align=left class="tg-yw4l">fd -t|--type -f foo</td>
<td class="tg-yw4l">Find for file type only.</td>
</tr>
 <tr>
<td align=left class="tg-yw4l">fd -t|--type d -t|--type e foo</td>
<td class="tg-yw4l">Find for empty directories only.</td>
</tr>
 <tr>
<td align=left class="tg-yw4l">fd -a|--absolute-path foo</td>
<td class="tg-yw4l">Find in current directory showing the full path, the string name "foo", in parent|sub directories and files.</td>
</tr>
<tr>
<td align=left class="tg-yw4l">fd -e|--extension txt</td>
<td class="tg-yw4l">Find for a particular file extension.</td>
</tr>
<tr>
<td align=left class="tg-yw4l">fd -H|--hidden foo</td>
<td class="tg-yw4l">Find for hidden and ignored files.</td>
</tr>
</tbody>
</table>

fzf interactive searching🔎 :
`Ctrl+T`

>**Note** - More info on usage :

>     man fd

>     man fzf
#

</p>
 </details>

<details><summary><b>Smarter directory navigating</b> <img src="https://user-images.githubusercontent.com/18756975/201506739-b30571af-0223-4413-86a6-c6fb6a887ce3.png" width=15px height=20px></summary>

[commacd](https://github.com/shyiko/commacd)
 
A faster way to move around 

_**Install**_ :
```bash
curl -sSL https://github.com/shyiko/commacd/raw/v1.0.0/commacd.sh -o ~/.commacd.sh && \
  echo "source ~/.commacd.sh" >> ~/.bashrc
```

commacd exports three commands: forward(`,`) │ backward(`,,`) │ backward+forward(`,,,`)

_**Usage**_ :
| Description | commacd | command |
| :--:| :--: | :--: |
| Enter directories using| , des | | 
| abbreviations. | └─>  | cd Desktop |

| Description | commacd | command |
| :--:| :--: | :--: |
| Move through multiple directories| , u/l/ce | | 
| using abbreviations. | └─>  | cd /usr/local/Cellar |

| Description | commacd | options |
| :--:| :--: | :--: |
| Choose directories with names  | , d |  | 
| starting with same letter. |  0  |  Desktop   |
| (= multiple choices)       |  1  | Documents |
|  0, 1 or 2               | 2  | Downloads    |
 
| Description | commacd | command |
| :--:| :--: | :--: |
| Given two directories jdk7 and jdk8 | , ~/d/j*8 | | 
| on the Desktop, cd into jdk8 without hitting | └─>  | cd ~/Desktop/jdk8   |
| interactive mode (the one shown above).       |  | |

| Description | commacd | 
| :--:| :--: | 
| Go back previous directory | ,, .. |

Tab = Autocomplete

>**Note** - More info on usage :

>   [shyiko.com/commacd](https://shyiko.com/2014/10/10/commacd/)
 
# 
 
[zoxide](https://github.com/ajeetdsouza/zoxide)
 
It remembers which directories you use most frequently, so you can "jump" to them in just a few keystrokes.
 
<img src="https://user-images.githubusercontent.com/18756975/202857373-1317ab89-d787-4b11-b5b0-c0cd4ce154ab.gif" width=500px height=300px>

_**Install**_ :
```bash
sudo apt install zoxide
```
Open ~/.bashrc and add 
```
eval "$(zoxide init bash)"
```
_Restart terminal_
 
> **Note** - Other installation info - [github.com/ajeetdsouza/zoxide#installation](https://github.com/ajeetdsouza/zoxide#installation)
 
_**Usage**_ :
 ```bash
z foo              # cd into highest ranked directory matching foo
z foo bar          # cd into highest ranked directory matching foo and bar
z foo /            # cd into a subdirectory starting with foo

z ~/foo            # z also works like a regular cd command
z foo/             # cd into relative path
z ..               # cd one level up
z -                # cd into previous directory

zi foo             # cd with interactive selection (using fzf)

z foo<SPACE><TAB>  # show interactive completions (zoxide v0.8.0+, bash 4.4+/fish/zsh only)
```
 
>**Note** - More info on usage :

>   [Algorithm matching](https://github.com/ajeetdsouza/zoxide/wiki/Algorithm#matching)
 
#

</p>
 </details>
 
<br>

> [!NOTE]
> There are more alternative tools available out there that may better fit your needs.<br>
> Check out [Modern Unix](https://github.com/ibraheemdev/modern-unix) - A collection of modern/faster/saner alternatives to common unix commands.
