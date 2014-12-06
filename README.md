BVEC
====
BIT VECTOR(BVEC) that can store hex strings efficiently given the width of the bit array.
The program has an inbuilt parser that can be used to perform very basic operations on bit arrays
such as adding two BVECs and making a new BVEC by selection of bits from an existing BVEC.

On starting the program,a BEE> prompt will be shown.Use "exit" to exit the program.

Examples:
<ul>
<li>Definition of a BVEC
	(C width_of_the_bit_array hex_string)
	
	BEE>(C 12 abc)
	
	<ul>Rules
	<li>If the width is greater than bit represented in hex_string,zeros are padded at the front.</li>
	<li>If the width is smaller,the leading bits are dropped.</li>
	</ul>
</li>
<li>Adding two BVECs
	(add BVEC_definition BVEC_definition)
	BEE>(add (C 12 abc) (C 4 g))
</li>
<li>Select
	(select BVEC_definition lo_index hi_index)
	BEE>(select (C 12 abc) 0 4)
</li>
</ul>

This program was inspired from a question in the AP Grade Contest CS101 2014 held at IIT, Bombay.
