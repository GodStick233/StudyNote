# Unit 1.2 Boolean Functions Synthesis

How to contruting boolean funciton with truth table:

![How to contruting boolean funciton with truth table](https://github.com/GodStick233/StudyNote/raw/master/Build-a-computer/img/2.png)

- Any Boolean function can be represrted using an expression containing AND and NOT operations.
  
  #### Proof:
  
  (x OR y) = Not(Not(x) AND NOT(y))

#### NAND:

![](https://github.com/GodStick233/StudyNote/raw/master/Build-a-computer/img/3.png)

- Any Boolean functioon can be represented using an expression containing only NAND operations.
  
  #### Proof:
  
  1) NOT(x) = (x NAND x)
  
  2) (x AND y ) = NOT(x NAND y)
  
  one expression can do every thing!!!

# Unit 1.3 Logic Gates

![](https://github.com/GodStick233/StudyNote/raw/master/Build-a-computer/img/3.png)

# Unit 1.4 Hardware Description language

  

e.g: HDL code to contruting XOR chip:

```nand2tetris-hdl
CHIP Xor{
    IN a,b;
    OUT out;
    
    PARTS:
    Not(in = a, out = nota);
    Not(in = b, out = notb);
    And(a = a, b = notb, out = aAndNotb);
    And(a = nota, b = b, out = notaAndb);
    Or(a = aAndNotb, b = notaAndb);
}
```


