# EXPERIMENT-01: BUILDING LOGICAL CIRCUITS

## 1. Aim

To design, implement, simplify, and verify combinational logic circuits using Boolean algebra and digital logic gates.

## 2. Boolean Notation

Use the following notation throughout this experiment:

| Symbol | Meaning | Example |
|---|---|---|
| `!A` | NOT A | `!A` |
| `A & B` | AND | `A & B` |
| `A \| B` | OR | `A \| B` |
| `A ^ B` | XOR | `A ^ B` |
| `A XNOR B` | XNOR | `A XNOR B` |

**Important:** In these equations, `!` means NOT, `&` means AND, `|` means OR, and `^` means XOR. Parentheses determine the order of operations.

## 3. Advanced Boolean Equations

### Equation 1: Four-Input Sum-of-Products

```text
F1 = (!A & B & C)
   | (A & B & !D)
   | (!B & C & D)
   | (A & !C & D)
```

**Inputs:** A, B, C, D  
**Output:** F1  
**Challenge:** Simplify the expression and compare gate counts.

### Equation 2: Product-of-Sums Circuit

```text
F2 = (A | !B | C)
   & (!A | B | D)
   & (B | !C | !D)
```

**Inputs:** A, B, C, D  
**Output:** F2  
**Challenge:** Implement the circuit using NAND gates and verify functional equivalence.

### Equation 3: Nested Complement Logic

```text
F3 = !(
       ((! (A | B)) | (C & D))
       &
       (A | (!(B | C)))
     )
```

**Inputs:** A, B, C, D  
**Output:** F3  
**Challenge:** Apply De Morgan's theorems and implement the circuit using NAND and NOR gates.

### Equation 4: XOR-XNOR Combinational Circuit

```text
F4 = ((A XOR B) & (C XNOR D))
   | (!A & B & (C XOR D))
```

**Inputs:** A, B, C, D  
**Output:** F4  
**Challenge:** Compare an XOR/XNOR implementation with a basic-gate implementation.

### Equation 5: Five-Input Logic Function

```text
F5 = (A & B & !C)
   | (!A & D & E)
   | (B & C & !E)
   | (!B & C & D)
```

**Inputs:** A, B, C, D, E  
**Output:** F5  
**Challenge:** Generate and verify all 32 input combinations.

### Equation 6: Six-Input Mixed Logic

```text
F6 = ((A | B) & !(C | D))
   | ((C XOR E) & (D | G))
   | (!A & B & E)
```

**Inputs:** A, B, C, D, E, G  
**Output:** F6  
**Challenge:** Calculate gate count and logic depth. Verify all 64 input combinations.

### Equation 7: NAND-NOR Hybrid Logic

```text
F7 = (! (A & B) & !(C | D))
   | (!(A | C) & B & D)
```

**Inputs:** A, B, C, D  
**Output:** F7  
**Challenge:** Implement the function using NAND and NOR gates with any required input inversions.

### Equation 8: Six-Input Advanced Combinational Logic

```text
F8 = ((A XOR B) & (C XNOR D))
   | (!(A | B) & C & E)
   | (A & B & !(D | F))
```

**Inputs:** A, B, C, D, E, F  
**Output:** F8  
**Challenge:** Simplify the expression, design the circuit, and verify all 64 input combinations.

## 4. Experimental Procedure

1. Identify all input variables and the output.
2. Draw the logic circuit for each equation.
3. Implement the circuit in Logisim Evolution, Proteus, or a digital logic trainer kit.
4. Apply all possible input combinations.
5. Record the expected and observed outputs.
6. Simplify the Boolean expression using Boolean algebra.
7. Build the simplified circuit and compare gate counts.
8. Save the circuit diagrams, truth tables, and verification screenshots.

## 5. Truth Table Requirements

| Number of inputs | Required combinations |
|---:|---:|
| 4 | 16 |
| 5 | 32 |
| 6 | 64 |

Use this format to record the results:

| Inputs | Expected output | Observed output | Status |
|---|---|---|---|
| 0000 |  |  |  |
| 0001 |  |  |  |
| 0010 |  |  |  |
| ... |  |  |  |

Extend the table to include every input combination required by each equation.

## 6. Performance Analysis

For each circuit, record:

- Number of AND gates
- Number of OR gates
- Number of NOT gates
- Number of XOR/XNOR gates
- Total gate count
- Logic depth
- Functional equivalence before and after simplification

## 7. Expected Results (drop the screenshots of each equations circuit )
Equation 1
<img width="319" height="210" alt="Screenshot 2026-10-31 201851" src="https://github.com/user-attachments/assets/c8373c14-7bea-487c-909b-a6c015320d1d" />

Equation 2
<img width="306" height="179" alt="Screenshot 2026-10-31 202422" src="https://github.com/user-attachments/assets/6fa5714a-cda3-4364-afea-eeed52d4b9a1" />

Equation 3
<img width="224" height="122" alt="Screenshot 2026-10-31 203110" src="https://github.com/user-attachments/assets/d081b0ee-e5c3-4921-a80f-2e77f4a2ba1f" />

Equation 4
<img width="455" height="316" alt="Screenshot 2026-10-31 204422" src="https://github.com/user-attachments/assets/1dd2104b-2336-4616-8316-20da33e55684" />

Equation 5
<img width="405" height="373" alt="Screenshot 2026-10-31 210158" src="https://github.com/user-attachments/assets/398dab56-9eae-4571-8197-73a2638c2a48" />

Equation 6
<img width="428" height="327" alt="Screenshot 2026-10-31 211247" src="https://github.com/user-attachments/assets/06a6879e-0671-4847-8a34-28e102cc5614" />

Equation 7
<img width="396" height="293" alt="Screenshot 2026-10-31 205621" src="https://github.com/user-attachments/assets/36b34b44-a42d-4454-9253-5e7df78a6be6" />

Equation 8
<img width="425" height="333" alt="Screenshot 2026-10-31 211956" src="https://github.com/user-attachments/assets/3b70429b-5111-4f3a-b04b-377b1561203c" />

 
## 8. Result

The logic circuits are designed, implemented, and verified using Boolean algebra and digital logic gates. The original and simplified circuits are compared based on gate count and logic depth.
 
 
