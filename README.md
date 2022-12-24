# Syntax-Tree
This code defines a ##SyntaxTree class that has several methods for creating a syntax tree for a given expression and printing the tree to the console.

The ##create_syntax_tree method uses the ##ast.parse function to parse the given expression and create a syntax tree. 
The tree is an instance of the ##ast.AST class, which represents the root node of the tree.

The ##Output method takes a node in the syntax tree as input and prints its class name and a string representation of the node, using the ##ast.dump function.
It then recursively calls itself on each child node of the input node to print the entire tree.

The ##takeinput method prompts the user to enter an expression, and returns the expression as a string.

Finally, the code creates an instance of the ##SyntaxTree class, prompts the user to enter an expression, creates a syntax tree for the expression, and prints the tree to the console. For example, if the user enters the expression "2 + 3 * 4", the ##output will be:

Module: "Module(body=[Expr(value=BinOp(left=Constant(value=2, kind=None), op=Add(), right=BinOp(left=Constant(value=3, kind=None), op=Mult(), right=Constant(value=4, kind=None))))])"
