# Faux-Racket-Interpter

## This is a Faux-Racket-Interpreter using Monadic Binding 

Can be used to evaluate expressions and functions defintions. 

Here we assume that expressions have been tokenized.  

## Sample use 

data Ast = 
      Number Int
    | Bin Op Ast Ast
    | Fun String Ast
    | With (String, Ast) Ast
    | App Ast Ast
    | Set String Ast
    | Seq Ast Ast
    | Var String


interp :: Ast -> Env -> State Val
interp (ADD 1 2) Empty --> Empty (Numb 3) 


Feel free to use!! 
