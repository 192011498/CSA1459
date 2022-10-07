%{
int c=0;
int d=0;
%}
%%
[0-9] {c++;}
[-][0-9] {d++;}
%%
int yywrap(void){}
int main(char argc[],char *argv[]){
yyin=fopen(argv[1],"r");
yylex();
printf("%d,%d",c,d);
fclose(yyin);
}
