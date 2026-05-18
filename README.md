# Computer Architecture Final Project:

Design a 32-Bit CPU to perform assembly level commands

Assembly Code in the design:

lw  $4, 0($0)      # load first value | Binary: 100011 00000 00100 0000000000000000

lw  $5, 1($0)      # load second value | Binary: 100011 00000 00100 0000000000000001

beq $4, $5, 2      # if equal, skip add/store | Binary: 000100 00100 00101 0000000000000010

add $6, $4, $5     # add them | Binary: 000000 00100 00101 00110 00000 100000

j   6               # jump forward | Binary: 000010 00000000000000000000000110

sw  $6, 2($0)      # store result | Binary: 101011 00000 00110 0000000000000010
