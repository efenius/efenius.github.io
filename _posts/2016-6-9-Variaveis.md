---
layout: post
title: Variaveis de Ambiente
---

#!/bin/bash
######################################################
# Vinydimax - DBA
# efenius.github.io
# Configurando variaveis de ambiente
#
#
#
#
#
#####################################################


umask 022
EDITOR=vim;        export EDITOR
TERM=xterm;        export TERM
TEMP=/tmp;        export TEMP
TMPDIR=/tmp;        export TMPDIR

export ORACLE_SID=vn
export ORACLE_BASE=/u01/app/oracle
export ORACLE_HOME=/u01/app/oracle/product/11.2.0.1/db_1
export ORACLE_UNQNAME=vn

export NLS_LANG=AMERICAN_AMERICA.WE8ISO8859P1
#export LANG=us_EN.UFT-8

export ORACLE_OWNER=oracle
export ORACLE_TERM=xterm


export PATH=$ORACLE_HOME/bin:$ORA_CRS_HOME/bin:$PATH:/usr/local/bin
export LD_LIBRARY_PATH=$ORACLE_HOME/lib:$ORA_CRS_HOME/lib:/usr/local/lib:$LD_LIBRARY_PATH
export CLASSPATH=$ORACLE_HOME/JRE:$ORACLE_HOME/jlib:$ORACLE_HOME/rdbms/jlib

alias dba='sqlplus "/ as sysdba"'

