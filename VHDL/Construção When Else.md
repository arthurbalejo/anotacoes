[[VHDL]]

![[Pasted image 20240428195527.png]]

```
-- Curso de VHDL #10
-- Exemplo de multiplexador com 4 entradas de 1 bit
-- Autor: eu
-- Data: 28/04/2024

entity mux_4_1 is
	port (
		D0, D1, D2, D3  :    in  bit;
		S0, S1          :    in  bit;
		Y               :    out bit
		) ;
end mux_4_1;

architecture main of mux_4_1 is
	
	signal sel  :   bit_vector(1 downto 0):= "00";
	
begin
	
	sel <= S1 & S0;
	
	y <= D0 when sel = "00" else
		 D1 when sel = "01" else
		 D2 when sel = "10" else
		 D3;
	
end main ; --main 
```