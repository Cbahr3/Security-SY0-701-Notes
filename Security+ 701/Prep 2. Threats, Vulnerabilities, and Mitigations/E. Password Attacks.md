**Password Attacks** - password attacks undermine system and information security
- *Hash Function* - a mathematical function that converts a variable-length input into a fixed-length output, criteria includes:
	- It must produce a completely different output for each input
	- It must be computationally difficult to retrieve the input from the output
	- It must be computationally difficult to find two different inputs that generate the same output
		- *The Birthday Problem* - collisions become common with large samples, what are the odds two people in a room will share a birthday? - 100% with 367 people, 50% with only 23 people, 99.9% with 70 people
- Types of Password Attacks:
	- *Brute Force Attacks* - try all possibilities
		- *Dictionary Attacks* - try English words first
		- *Hybrid Attacks* - add variations to tries
		- *Rainbow Table Attack* - precomputes hashes

**Password Spraying and Credential Stuffing**
- *Password Spraying* - exploits common passwords, prohibit the use of common passwords
- *Credential Stuffing* - exploits reused passwords, use a password manager to generate and maintain unique passwords
- *Multi-factor Authentication* - stops password spraying and credential stuffing attacks