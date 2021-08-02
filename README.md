# seq-weighting 

## Description
- A program that calculates sequence weighting in Multiple Sequence Alignment.
- It supports two types of weighting, position-based method[1] and distance-based method[2].

## Compilation 
You can compile the program with `Cargo`. 🦀📦

[e.g.]

``` 
% cd seq-weighting-main
% cargo build --release
``` 

Then the object file will be generated in `./target/release` directory. 

## Input file format 
Aligned Multi-FASTA format in amino acid sequences.  
See sample files in `demo` directory. 

## Usage 
- `-i` : Input file name, REQUIRED.
- `-o` : Output file name, REQUIRED.
- `-m` : Method of weighting, position-based or distance-based. 

[e.g.]

```
% ./seq-weighting -i input.fasta -o output.txt -m va 
``` 
Type `-h` to see other available options.

## Output 

[e.g.]
<img width="1036" alt="image_res" src="https://user-images.githubusercontent.com/83740080/122624713-7e94de00-d0dc-11eb-8565-35bdbf161432.png">

## References 

1. Henikoff, Steven, and Jorja G. Henikoff. "Position-based sequence weights." Journal of molecular biology 243.4 (1994): 574-578.
2. Vingron, Martin, and Patrick Argos. "A fast and sensitive multiple sequence alignment algorithm." Bioinformatics 5.2 (1989): 115-121.
