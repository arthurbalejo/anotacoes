[[VHDL]]
````
-- curso VHDL #3
-- Exemplo somador 4bits
-- Autor: arthur
-- Data: 22/04/2024

entity somador is
	port(
		a, b    :   in    integer range 0 to 15;
		z       :   out   integer range 0 to 15
	);
end somador;

architecture main of somador is
begin
	z < = a + b;
end main;
```