---
layout:  post
title:	vim ��װyoucompleteme
---

### ��װgit��zsh
��װzsh��Ҫ�õ�git,���Ե�һ���ǰ�װgit ��zsh 
```
sudo apt-get install git zsh
```
### ʹ�ýű���װoh-my-zsh
```
$ sh -c "$(wget https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
```
### ��������Ͳ��
Ĭ�ϵ�����Ͳ���� "robbyrussel" 
�������ʹ�� `echo $ZSH_THEME`���Կ��ĵ�
���������� .zshrc��,��ʾΪ`ZSH_THEME="robbyrussel"`
����������˺ö������,�������ǰ������������Ϊ���,ÿ�ο��ն˾Ͳ�һ����.
���ǿ��԰������Ϊ`ZSH_THEME="random"` ֮��,ѡ��ú��õ������Ժ�,ʹ��`echo $ZSH_THEME`�鿴�������Ǹ�����,Ȼ�����`.zshrc`�е�`ZSH_THEME=xxxxx`����,����xxxxxxΪ���������.���漴��. ʹ��source .zshrc ��ʹ�����������û�������������Ч.

Ĭ�ϵĲ���� `git`ֻ���������,�����Ĳ����.oh-my-zsh���ļ��ĵ�plugins�����кö������Բ鿴 oh-my-zsh�����Ŀ���鿴.
