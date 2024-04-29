[[VHDL]]
```
-- curso VHDL #2
-- Exemplo porta and
-- Autor: arthur
-- Data: 24/04/2024

entity somador_completo is
	port(
		A, B    :   in  bit; --entradas
		TE      :   in  bit; -- Transporte de entrada
		S       :   out bit; -- soma
		TS      :   out bit  -- soma
	);
end entity;

architecture main of somador_completo is begin
    S < = A xor B xor TE;
    TS < = (A and B) or (A and TE) or (B and TE);
end architecture:
-- fim
```