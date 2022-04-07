
#To build the .java and .lex files

./build.sh


# To parse, give the input file and specify an output file. exec.sh handles the scanning and Parsing
# An output.scan file will be created by the scanner to use as input for the parser

./exec.sh <inputfile.decaf> <outputfile>

# There will probably be some extra lines because some text is not aligned such as `(actuals) FieldAccess` will be on different lines but the parsing is still correct

#Unfortunetaly I did not have enough time to implement error handling for syntax and other errors but the parser does parse the sample decaf files correctly. If a program does not  follow the grammer then the program will just stall and spit out any output
