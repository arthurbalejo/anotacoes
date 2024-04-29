[[VHDL]]
````
-- curso VHDL #2
-- Exemplo porta and
-- Autor: arthur
-- Data: 22/04/2024

-- Bibliotecas e pacotes

-- Entidade
entity and_gate is
	port(
		a, b    :    in  bit;
		z       :    out bit
	);
end entity and_gate;

-- Arquitetura
architecture main of and_gate is
begin
	z < = a and b;
end architecture main:

-- Configuração
```