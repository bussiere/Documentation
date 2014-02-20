Date: 2014-02-20
Title: Erlang
Category: Geek
Tags: erlang


Un helloworld en erlang hello.erl

	-module(hello).
	-export([hello_world/0]).

	hello_world() -> io:fwrite("hello, world\n").


Quelques commandes utiles pour erlang :

Compiler le fichier erl :

	erlc hello.erl

executer hello_world dans hello.erl :

	erl -noshell -s hello hello_world -s init stop	
