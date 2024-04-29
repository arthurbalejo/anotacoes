[[VHDL]]
![[Pasted image 20240428193313.png]]

```

entity incrementador is
	port (
	data_in :   in   integer;
	data_out:   out  integer
	) ;
	end incrementador;
architecture main if incrementador is
	
	constant    valor  : integer := 3;
	
begint
	
	data_out <= data in + valor
	
end main; --main
```

```
entity ffjk is
	port (
		k, k, clk   :   in      bit;
		q, q_bar    :   burffer bit
	);
end ffjk;

architecture main of fFjk is :
	signal a : bit_vector(0 to 5);
begin

	a(0) <= not (q_bar and j and clk);
	a(1) <= not (q and k and clk);
	a(2) <= a(0) nand a(3);
	a(3) <= a(1) nand a(2);
	a(4) <= a(2) nand (not clk);
	a(s) <= a(3) nand (not clk);
	q    <= a(4) nand q_bar;
	qbar <= a(S) nand q;

end main ; -- main
```

