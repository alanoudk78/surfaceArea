# surfaceArea
example float surface Area by MIPS 

.data
surfaceArea: .float 0.0
pi: .float 3.14
readius: .float 3.0
num1: .float 4.0


.text
l.s $f4,pi
l.s $f6,readius
l.s $f12,num1
mul.s $f8.$f6,$f6
mul.s $f10,$f8,$f4
mul.s $f11,$f10,$f12
s.s $f11,surfaceArea

li $v0,10
syscall
