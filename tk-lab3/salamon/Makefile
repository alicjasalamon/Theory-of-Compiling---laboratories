all: salamon_aksamit

salamon_aksamit: salamon_aksamit.tab.c lex.yy.c
	gcc -g -o salamon_aksamit salamon_aksamit.tab.c lex.yy.c	

salamon_aksamit.tab.c: salamon_aksamit.y
	bison -d salamon_aksamit.y

lex.yy.c: salamon_aksamit.l
	flex salamon_aksamit.l

clean: 
	rm salamon_aksamit salamon_aksamit.tab.c salamon_aksamit.tab.h lex.yy.c
