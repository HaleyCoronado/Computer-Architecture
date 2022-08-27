Read Me

1) Haley Coronado (RedID 824874564)

2) 
	HCoronado2.clf
		This is the library file. It contains the subcircuits used in the final circuit (ECC
		Generator, 13-bit Data Transmission, and Main Memory).
			ECC Generator: takes an 8-bit data vector from the I/O Controller and generates
			13-bit vecotr by interalcing a 4-bit parity vector. The ECC Generator appends an
			additional parity bit to the 12-bit hamming code to ensure even parity.
			13-bit Data Transmission: a 13-bit bus line to send the 8-bit binary data and 5
			parity bits over to memory. The 13-bit Data Transmission also has an additonal
			13 bits of input for simulating errors.
			Main Memory: contains an ECC Detector to correct single bit errors, and determine
			how many errors occured.
		
	Lab2.cct
		This is the final circuit that combines all of the subcircuits to create the system
		for the transmission of 8-bit packets from an I/O Controller to Memory, using error
		correcting code over a 13-bit bus line.
